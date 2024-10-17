# **Web Servers:**
  ## Apache HTTPD

### 1. **Apache HTTPD Installation and Basic Configuration**
   - Install Apache HTTPD (`yum install httpd`).
   - Start and enable the Apache service (`systemctl start httpd` and `systemctl enable httpd`).
   - Configure Apache to serve a simple HTML page and verify it using `curl` or a web browser.

### 2. **Virtual Hosts Configuration**
   - Create and configure multiple virtual hosts to serve different websites on the same server.
   - Use name-based virtual hosting to run multiple websites from a single IP address.
   - Set up separate document roots and log files for each virtual host.

### 3. **Securing Apache with SSL/TLS**
   - Install `mod_ssl` and configure Apache to support HTTPS.
   - Generate a self-signed SSL certificate or use a trusted certificate authority (CA).
   - Modify the Apache configuration to enable HTTPS and redirect all HTTP traffic to HTTPS.
   - Test your HTTPS setup using a browser or tools like `curl`.

### 4. **Apache User Authentication**
   - Set up basic authentication using `.htpasswd` files.
   - Restrict access to certain directories on your website by requiring a username and password.
   - Configure Digest Authentication for more secure credential storage.

### 5. **Custom Error Pages**
   - Configure Apache to display custom error pages (e.g., `404 Not Found`, `403 Forbidden`).
   - Create your own HTML pages for each error code and configure Apache to use them.

### 6. **Enabling Directory Listings**
   - Enable directory listing for a specific directory in the Apache configuration.
   - Customize the look and feel of the directory listing with `mod_autoindex`.
   - Secure the directory listing with user authentication.

### 7. **Setting Up Aliases and Redirects**
   - Use `Alias` directives to serve files from different directories.
   - Configure URL redirects using `Redirect` or `RewriteRule` (from `mod_rewrite`).
   - Set up both temporary (`302`) and permanent (`301`) redirects for different pages.

### 8. **Apache Logging**
   - Configure and manage Apache logs (access and error logs).
   - Set up custom log formats to capture specific information (e.g., client IPs, response times).
   - Use log rotation with `logrotate` to manage large log files.

### 9. **Configuring Apache Modules**
   - Enable and configure various Apache modules (`mod_rewrite`, `mod_proxy`, `mod_ssl`).
   - Understand how to load and unload modules and manage module configurations.

### 10. **Apache Performance Tuning**
   - Tune the `MaxClients`, `StartServers`, and `KeepAlive` settings to optimize performance.
   - Configure caching with `mod_cache` and test its effects.
   - Enable compression using `mod_deflate` to improve page load times.

### 11. **Serving Dynamic Content with PHP**
   - Install and configure PHP to work with Apache HTTPD (`yum install php`).
   - Create a simple PHP script and serve it using Apache.
   - Test the integration of Apache and PHP by running dynamic web pages.

### 12. **Reverse Proxy with Apache HTTPD**
   - Use `mod_proxy` to configure Apache as a reverse proxy server.
   - Set up Apache to pass incoming requests to backend servers (e.g., Nginx or a Tomcat server).
   - Implement load balancing across multiple backend servers.

### 13. **Securing Apache with SELinux**
   - Configure Apache to run under SELinux in enforcing mode.
   - Learn how to troubleshoot and resolve common SELinux-related issues with Apache.
   - Use `semanage` and `chcon` to adjust SELinux contexts for files served by Apache.

### 14. **Access Control with Apache**
   - Use `Allow`, `Deny`, and `Require` directives to control access to your website.
   - Set up IP-based access control to restrict or allow access based on client IP addresses.

### 15. **Setting Up Apache as a Load Balancer**
   - Use `mod_proxy_balancer` to configure Apache as a load balancer.
   - Set up round-robin load balancing to distribute traffic across multiple backend servers.
   - Test failover scenarios by shutting down one of the backend servers and observing behavior.

### 16. **Configuring Apache for High Availability**
   - Integrate Apache with HAProxy or a similar load balancer for high availability.
   - Set up session persistence and sticky sessions to maintain user sessions across multiple servers.

### 17. **Rate Limiting with Apache**
   - Configure Apache to limit the number of requests a client can make per second (`mod_ratelimit`).
   - Implement rate limiting on specific URLs or directories to prevent abuse.



