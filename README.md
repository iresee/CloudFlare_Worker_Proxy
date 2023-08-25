# CloudFlare_Worker_Proxy
利用CloudFlare Worker代理网站，下面是一些说明：
// Website you intended to retrieve for users.将要代理的的网站，这里以谷歌为例。
const upstream = 'www.google.com'

// Custom pathname for the upstream website.上游网站的自定义路径名，填入自己的网址。
const upstream_path = '/'

// Website you intended to retrieve for users using mobile devices.将要代理的的手机网站，这里依然以谷歌为例。
const upstream_mobile = 'www.google.com'

// Countries and regions where you wish to suspend your service.暂停服务的国家和地区，填入你不想服务的地区。
const blocked_region = ['CN', 'KP', 'SY', 'PK', 'CU']

// IP addresses which you wish to block from using your service.阻止服务的 IP 地址，填入即可组织相应的IP地址访问。
const blocked_ip_address = ['0.0.0.0', '127.0.0.1']

// Whether to use HTTPS protocol for upstream address.是否启用 HTTPS 协议。
const https = true

// Whether to disable cache.是否禁用缓存。
const disable_cache = false
