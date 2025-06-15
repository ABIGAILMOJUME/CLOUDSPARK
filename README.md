# 🚀 CloudSpark - Smart Infrastructure Revolution


## 📋 Project Overview
 This project demonstrates a full-stack web application deployed on a cloud provider, featuring a dynamic landing page that would make even the most seasoned DevOps engineer shed a single, proud tear.

**Project Title:** "CloudSpark - Igniting the Future of Smart Infrastructure"  
**Developer:** Abigail Mojume{My humble self}  
**Reality Check:** *It's a very basic landing page, but it's MY professionally deployed landing page*
 

### Project Components
1. **Server Provisioning**: Spun up a cloud instance faster than you can say "infrastructure as code"(because who has time for physical servers in 2025?)
2. **Web Server Configuration**: Nginx setup with reverse proxy capabilities
3. **Domain & DNS**: Custom domain pointing to the cloud instance
4. **SSL Implementation**: HTTPS because security matters 
5. **Production-Ready Deployment**: Because localhost is for quitters


## 🔧 Deployment Process

### Phase 1: Server Setup
1. Provisioned an EC2 instance on AWS
2. Configured initial security (SSH keys, firewall rules)
3. Updated system packages (because security updates wait for no one)

### Phase 2: Web Server Configuration
1. Installed and configured Nginx
2. Set up server blocks for domain handling
3. Configured reverse proxy settings
4. Tested initial deployment

### Phase 3: Content Deployment
1. Created a functional landing page
2. Optimized assets for production
3. Deployed files to web server directory
4. Configured proper file permissions

### Phase 4: Domain & SSL
1. Configured DuckDNS for dynamic DNS management
2. Battled with SSL certificate implementation (and won, eventually)
3. Used manual certificate generation when automation failed
4. Implemented HTTPS redirects for secure connections

### Phase 5: Production Hardening
1. Configured firewall rules (HTTP/HTTPS only)
2. Final testing and optimization

## 🧰 Technologies Used

- **Frontend**: HTML, CSS.
- **Web Server**: Nginx
- **Operating System**: Ubuntu 20.04 LTS
- **Cloud Provider**: AWS
- **SSL/TLS**: HTTPS security implementation
- **DNS**: DuckDNS dynamic domain management



### Challenges Faced
Let's Encrypt decided to be... let's call it "particular" about automatic certificate generation. Standard `certbot` commands were throwing more errors than a JavaScript framework on release day.

### The Solution
When automation fails, we get creative:
```bash
# The nuclear option that actually worked
sudo certbot certonly --manual --preferred-challenges dns -d yourdomain.com
```
This command bypassed the automatic verification and allowed manual DNS challenge completion. Sometimes you have to tell the robots exactly what to do, and this time, the robot listened.




## 📱 Live Demo

**Live Site**: https://semester2exam.duckdns.org/  
**Status**: ✅ Fully operational and publicly accessible



## 📸 Project Screenshot

![SEMESTER2EXAM](https://github.com/user-attachments/assets/9dca3662-24e9-4b48-a5fd-82ad4253dbc7)
*Functional landing page showcasing CloudSpark's intelligent cloud infrastructure vision*



