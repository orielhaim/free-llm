# Free-LLM

i bought/rented a frankly irresponsible amount of inference hardware and most of it is just sitting there.

so you can use it for free. please use it for good things.

star this repo, then use your github username as the api key. you get 100 requests an hour, which feels generous.

```ts
import OpenAI from "openai";

const client = new OpenAI({
  baseURL: "https://inf3.orielhaim.com/v1",
  apiKey: "your-github-username",
});

const result = await client.responses.create({
  model: "kimi-k3",
  input: "hello",
});
```

go wild.
