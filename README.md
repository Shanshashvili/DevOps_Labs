# **Web Server:**
## Nginx

### 1. **NGINX Installation and Basic Configuration**
   - Install NGINX (`yum install nginx`).
   - Start and enable the NGINX service (`systemctl start nginx` and `systemctl enable nginx`).
   - Configure NGINX to serve a static HTML page and verify using `curl` or a web browser.
   - Learn about the structure of NGINX configuration files (global context, HTTP, server, and location blocks).

### 2. **Serving Static and Dynamic Content**
   - Serve both static files (HTML, CSS, JS) from a directory.
   - Configure NGINX to serve dynamic content using a backend server (e.g., PHP-FPM or a Python app).
   - Test serving PHP with NGINX using `php-fpm` and configure the location block for `.php` files.

### 3. **Virtual Hosts Configuration**
   - Set up multiple server blocks (virtual hosts) to host multiple websites on the same NGINX instance.
   - Use both name-based and IP-based virtual hosting.
   - Configure separate document roots and error logs for each virtual host.

### 4. **Configuring SSL/TLS for HTTPS**
   - Enable HTTPS on NGINX by configuring SSL using a self-signed certificate or a trusted certificate authority (CA).
   - Modify your NGINX configuration to support SSL and redirect all HTTP traffic to HTTPS.
   - Use tools like `openssl` or `certbot` to manage your certificates.
   - Ensure strong SSL/TLS security by disabling weak ciphers and enforcing TLS 1.2+.

### 5. **NGINX Reverse Proxy**
   - Configure NGINX as a reverse proxy to pass client requests to backend servers (e.g., Apache, Node.js).
   - Set up a simple reverse proxy by forwarding requests to an upstream server.
   - Test load balancing and failover features by configuring multiple backend servers.

### 6. **NGINX Load Balancing**
   - Implement load balancing across multiple backend servers using the `upstream` block.
   - Experiment with different load balancing methods (`round-robin`, `least_conn`, `ip_hash`).
   - Test failover scenarios by stopping one of the backend servers and observing NGINX's behavior.

### 7. **Securing NGINX with Basic Authentication**
   - Set up HTTP Basic Authentication to protect certain resources or directories.
   - Use the `htpasswd` command to create password files for user authentication.
   - Secure sensitive paths like `/admin` using password authentication.

### 8. **Configuring NGINX as a Web Application Firewall (WAF)**
   - Use `ModSecurity` or NGINX's `ngx_http_access_module` to block malicious traffic.
   - Set up rate limiting, connection limiting, and request filtering to protect against DDoS attacks and other security threats.
   - Configure rules to block specific user agents or referrers.

### 9. **URL Rewriting and Redirects**
   - Use the `rewrite` directive to rewrite URLs for better SEO or URL structure.
   - Implement 301 (permanent) and 302 (temporary) redirects to move pages or websites.
   - Use `try_files` for cleaner and more efficient handling of URL routing.

### 10. **NGINX Caching**
   - Enable and configure content caching with `proxy_cache` for reverse-proxy setups.
   - Fine-tune cache expiration times and storage settings for specific file types or routes.
   - Test cache behavior using tools like `curl` to verify cache hits and misses.

### 11. **Gzip Compression**
   - Enable and configure gzip compression to optimize data transfer sizes.
   - Set up conditional gzip based on file types (e.g., compress HTML, CSS, JS but not images).
   - Analyze the effects of gzip compression on performance using tools like `curl` or browser developer tools.

### 12. **NGINX Logging and Log Analysis**
   - Configure access and error logs for NGINX.
   - Set up custom log formats to include additional data like response time, request headers, etc.
   - Use log analysis tools like `GoAccess` or `grep` to monitor traffic patterns and detect issues.

### 13. **Setting Up NGINX as a Content Delivery Network (CDN)**
   - Use NGINX to cache static assets close to users for faster access.
   - Set up cache expiration policies for static files.
   - Test the CDN setup with image, CSS, and JavaScript resources to see load time improvements.

### 14. **Handling Large File Uploads**
   - Configure NGINX to handle large file uploads by modifying the `client_max_body_size` directive.
   - Set up appropriate timeouts for handling long-running file uploads.

### 15. **Monitoring and Performance Tuning**
   - Use `stub_status` or NGINX's Prometheus exporter to monitor server metrics like active connections and request rates.
   - Tune worker processes, buffer sizes, and timeout settings for optimal performance.
   - Load test your NGINX server using `ab` (ApacheBench) or `wrk` to measure its performance under heavy load.

### 16. **FastCGI and PHP-FPM Configuration**
   - Install and configure `php-fpm` to handle PHP processing with NGINX.
   - Use the `fastcgi_pass` directive to forward PHP requests to PHP-FPM.
   - Optimize FastCGI parameters like `fastcgi_cache` and `fastcgi_buffer_size` for better performance.

### 17. **Securing NGINX with SELinux**
   - Ensure that NGINX runs under SELinux in enforcing mode.
   - Resolve common SELinux-related issues that might arise while serving files or running PHP-FPM.
   - Adjust SELinux contexts for NGINX’s document root and log files.

### 18. **NGINX Access Control**
   - Use `allow` and `deny` directives to restrict access based on IP addresses.
   - Configure access control to limit or block traffic from specific IP ranges or countries using `geo` module.

### 19. **High Availability NGINX with Keepalived**
   - Set up NGINX with Keepalived to provide high availability and failover for your web server.
   - Configure virtual IP addresses (VIP) that automatically move between NGINX instances during failover.
   - Test failover scenarios by bringing down one NGINX instance.
