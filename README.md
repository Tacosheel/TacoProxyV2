# [TacoProxy V2](https://proxy.tacosheel.dev)
### A node.js web proxy for use in combating web filters

# Updates
```
(Updated 9/28/21): TacoProxy V2 will not be updated. Subject to change at anytime.
```
# Security
### VirusTotal:
#### [beta.tacosheel.dev | 9/28/21](https://www.virustotal.com/gui/url/af2040df6606512662fb37fe02ff9a4914b0a384c19ed4cbc100613600785a5c/detection)

### SSL/TLS:
Taco Proxy is encrypted with the latest TLS 1.3

Since Heroku does not support SSL Certificates for free dynos, the next best alternative is using CloudFare Flexible.

### Email Address Obfuscation
CloudFare will attempt to obfuscate email addresses on Taco Proxy to prevent harvesting by bots and spammers

# Speed
There a lot of speed improvements since Aero Proxy, mainly including:

- Brotli Compression
- Rocket Loader
- Auto Minify
- Cloudfare Caching
- Arc.io Caching
- Browser Cache

##### PageSpeed rating of [100/100](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fbeta.tacosheel.dev%2F&tab=desktop) 

# Domains
#### [beta.tacosheel.dev](https://beta.tacosheel.dev)

# Deploy
<a href="https://heroku.com/deploy?template=https://github.com/Tacosheel/TacoProxyV2" title="Deploy to Heroku"><img alt="Deploy to Heroku" src="https://www.herokucdn.com/deploy/button.svg" width="140" height="30"><img></a>
&nbsp;

## Running locally

```sh
git clone https://github.com/titaniumnetwork-dev/alloyproxy.git
cd alloyproxy
node server.js
```

## Options in config.json
```json
{
    "port": "8080",
    "ssl": false,
    "prefix": "/web/",
    "localAddresses": [],
    "blockedHostnames": []
}
```

`"port": "8080"` = Sets HTTP server port of web proxy.

`"ssl": "false"` = Sets HTTP server SSL.

`"prefix": "/web/"` = Sets the overall prefix of the web proxy.

`"localAddresses": [ "0.0.0.0" ]` = Allows you to choose which IP to make the request from. If there are multiple IP's then the IP chosen will be randomized.

`"blockedHostnames": [ "example.org", "example.com" ]` = If the hostname of the proxy URL matches any of the URL hostnames listed in the array, the request to the server will be cancelled.

# Credits
- [Titanium Network](https://github.com/titaniumnetwork-dev)
- [QuiteAFancyEmerald](https://github.com/QuiteAFancyEmerald)
- [Jason](https://github.com/caracal-js)
- [B3ATDROP3R](https://github.com/B3ATDROP3R)
- [shirt](https://github.com/shirt-dev)
- [Xproassassinn](https://github.com/Xproassassinn)

# License 
![GitHub](https://img.shields.io/github/license/Tacosheel/TacoProxyV2)
```
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
### Copyright (c) 2021 Tacosheel
