## Examples
### OPENAI_API_KEY
```
export OPENAI_API_KEY=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
```
### Simple prompting
```
openai api chat.completions.create -m gpt-3.5-turbo -g user "What is the best way to loose weight"
```
### Generate an image
URL=$(openai api images.generate -p "An imaginary devops and kubernetes world" | jq -r '.data[0].url')
curl -O $URL
