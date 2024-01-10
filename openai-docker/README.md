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
