# Gemini-proxy

- gemini-proxy-cloudflare

## 这是利用cloudflare的work.js反向代理google的gemini的API接口

- [参考官方Gemini文档](https://ai.google.dev/tutorials/rest_quickstart)

## 使用方式

- 部署**work.js**到cloudflare
- 配置work触发器，定义域名

## 官方使用示例

```shell
curl https://generativelanguage.googleapis.com/v1beta/models/gemini-pro?key=$API_KEY
```

## cloudflare反代后的使用示例

```shell
curl https://gemini.aivvm.com/v1beta/models/gemini-pro?key=$API_KEY
```

## Deployment

Click the button below to deploy this worker to your Cloudflare account:

[![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/netcookies/Gemini-proxy)

## Local Development

1. Install Wrangler:
```bash
npm install -g wrangler
```

2. Login to your Cloudflare account:
```bash
wrangler login
```

3. Start the development server:
```bash
wrangler dev
```

## Manual Deployment

Deploy to Cloudflare Workers using Wrangler:

```bash
wrangler deploy
```

## License

MIT
