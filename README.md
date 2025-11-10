# Image Watermark Tool
Image Watermark Tool 是一個開源項目，使用者可以在本地設備上給自己的圖片（如身份證、駕照、護照等）添加浮水印，無需任何網路連接，並具有輕鬆的一鍵網站部署功能。
👉 [Image Watermark Tool](https://watermark.aicompasspro.com)

[English](https://github.com/unilei/image-watermark-tool/blob/master/README.EN.md) | [簡體中文](https://github.com/unilei/image-watermark-tool/blob/master/README.CN.md) | 正體中文

## 快速開始

### 在 Vercel 上部署
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/unilei/image-watermark-tool.git&project-name=image-watermark-tool&repository-name=image-watermark-tool)

### 在 Vercel 上手動部署 操作方法

```
1. fork 本項目
2. 在 [Vercel] 官網點擊 [New Project]
3. 點擊 [Import Git Repository] 並選擇你 fork 的此項目並點擊 [import]
4. 然後直接點 [Deploy] 接著等部署完成即可
```

### 1. 克隆項目

```bash
git clone https://github.com/unilei/image-watermark-tool.git
```

### 2. 安裝依賴
```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install
```
### 3. 運行到流覽器

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev
```

### 4. 在流覽器打開 [http://localhost:3001](http://localhost:3001)
![success_deploy.jpg](https://www.aicompasspro.com/api/imghosting/file/fddc13c78a10d7f841ac1.png)

#### 如何部署到自己伺服器？ NUXT.JS 打包部署文檔
[部署文檔](https://nuxt.com/docs/getting-started/deployment)

### 如何通過 Docker 部署

### 1. 方式一
```bash
docker pull ghcr.io/chung1912/image-watermark-tool:master
```

```bash
docker run -it --name image-watermark-tool \
-p 3000:3000 \
--restart always \
ghcr.io/chung1912/image-watermark-tool:master
```

### 2. 方式二
```bash
docker pull ghcr.io/chung1912/image-watermark-tool-nginx:master
```

```bash
docker run -it --name image-watermark-tool-nginx \
-p 8080:80 \
-p 8443:443 \
-v /path/to/private.pem:/etc/nginx/private.pem  \
-v /path/to/private.key:/etc/nginx/private.key \
--restart always \
ghcr.io/chung1912/image-watermark-tool-nginx:master
```
