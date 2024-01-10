## Building a container image to test OpenAI
```
docker build -t xxradar/openai-cli .
```
Make sure to have OPENAI_API_KEY set
```
export OPENAI_API_KEY=sk-xxxxxxxxxxx
```
```
docker run -it -e OPENAI_API_KEY=$OPENAI_API_KEY xxradar/openai-cli 
```
```
docker run -it -e OPENAI_API_KEY=$OPENAI_API_KEY xxradar/openai-cli \
          openai api chat.completions.create \
          -m gpt-3.5-turbo \
          -g user "What is the best way to loose weight"
```
