# Automatic Build of Dynamic NGINX Modules

This project is designed for automatic compilation and distribution of ready-to-use **dynamic modules** for the NGINX web server.

## 📦 Ready-to-Use Builds

You don't need to compile modules yourself — all build artifacts are available for download on the project's **[releases page](https://github.com/iperon-net/nginx-module/releases)**.

## 🔧 Project Components (Available Modules)

Currently, the project automatically builds the following popular third-party modules:

- **[ngx_http_geoip2_module](https://github.com/leev/ngx_http_geoip2_module)** (leev/ngx_http_geoip2_module) — module for determining client geographic location by IP address (based on GeoIP2 databases).
- **[headers-more-nginx-module](https://github.com/openresty/headers-more-nginx-module)** (openresty/headers-more-nginx-module) — module for flexible management of request and response headers (set, add, delete, modify).
- **[redis2-nginx-module](https://github.com/openresty/redis2-nginx-module)** (openresty/redis2-nginx-module) — module for direct communication with Redis server from NGINX configuration.
- **[xss-nginx-module](https://github.com/openresty/xss-nginx-module)** (openresty/xss-nginx-module) — module for Cross-Site Scripting (XSS) filtering and processing.

## ✨ Project Features

- **Automation:** Builds are triggered automatically when new NGINX versions are released.
- **Up-to-date:** Modules are compiled for the latest **stable** and **mainline** versions of NGINX.
- **Convenience:** Simply download the ready `.so` file matching your version and operating system, then enable it in your configuration.

## 🚀 Usage

1. Go to the **[Releases section](https://github.com/iperon-net/nginx-module/releases)**.
2. Select the required NGINX version and build type (mainline/stable).
3. Download the archive containing the modules.
4. Extract the module files (typically with `.so` extension) to your NGINX modules directory (e.g., `/etc/nginx/modules/`).
5. Enable the modules in your main `nginx.conf` configuration file using the `load_module` directive.

---

*Note: The project is under active development, and the list of supported modules may expand over time.*