# cloudflare-cors-proxy

A simple CORS proxy that can easily be uploaded as a Cloudflare Worker.

The worker proxies a request through the cloudflare worker. This allows you to get around CORS restrictions in browsers,
without changing the CORS settings of a server.

> Because CORS proxies are often used for nefarious things, of which I would not like to be a part of, I won't post a
> link to a working CORS proxy here, but they're easy to create in cloudflare without installing anything, and they're
> available on the free tier.

## Usage

Just put the URL you'd like to proxy to where `$TARGET_URL` is in the string below.

`curl "https://corsproxy.$CLOUDFLARE_USER.workers.dev/corsproxy/?apiurl=$TARGET_URL"`


![](https://user-images.githubusercontent.com/1910070/107144320-7a73db00-6908-11eb-9463-c33cccb8e64c.png)
