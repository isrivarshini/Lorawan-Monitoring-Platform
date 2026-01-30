# 🚀 Choovio IoT Platform

A modern, enterprise-grade IoT platform built on Magistrala with custom React frontend and AWS deployment capabilities.

![Choovio Logo](Frontend/public/assets/logo1.webp)

## 📋 Project Overview

The Choovio IoT Platform is a comprehensive pilot project demonstrating:
- **Modern IoT Infrastructure**: Built on the robust Magistrala platform
- **Custom Branding**: White-label solution with Choovio branding
- **Enterprise Frontend**: React + TypeScript admin dashboard
- **Cloud-Ready**: Production AWS deployment with auto-scaling
- **AI-Assisted Development**: Extensively documented AI usage throughout

---

## 🏗️ Project Structure

```
magistrala/
├── Backend/              # Magistrala IoT platform (Go)
├── Frontend/             # React admin dashboard (TypeScript + Vite)
├── Docker/               # Local development containers
├── aws-deployment/       # AWS infrastructure (Terraform)
│   ├── terraform/        # Infrastructure as Code
│   ├── scripts/          # Deployment automation
│   └── docs/             # AWS deployment guides
├── PROJECT_REPORT.md     # Comprehensive project documentation
└── README.md             # This file
```

---

## ⚡ Quick Start (Local Development)

### Prerequisites
- Docker & Docker Compose
- Node.js 18+
- npm or yarn

### 1. Start Backend Services
```bash
cd Docker
docker-compose up -d
```

### 2. Start Frontend Dashboard
```bash
cd Frontend
npm install
npm run dev
```

### 3. Access the Application
- **Dashboard**: http://localhost:5173
- **Backend API**: http://localhost:9000

### Demo Credentials
- **Email**: admin@example.com
- **Password**: 12345678
- **Role**: Admin (Full access)
---


## 🎨 Features

### Frontend Dashboard
- **Modern UI**: React + TypeScript with Tailwind CSS
- **Responsive Design**: Works on desktop, tablet, and mobile
- **User Management**: Full CRUD operations with role-based access
- **Device Management**: Monitor and manage IoT devices
- **Channel Management**: Configure communication channels
- **Health Monitoring**: Real-time system health checks
- **Demo Mode**: Works offline with mock data

### Backend Integration
- **Magistrala Platform**: Open-source IoT infrastructure
- **RESTful APIs**: Standard HTTP APIs for all operations
- **PostgreSQL Database**: Reliable data persistence
- **Docker Containerized**: Easy deployment and scaling
- **Authentication**: JWT-based secure authentication

### Branding & Customization
- **White-Label Ready**: Custom Choovio branding
- **Logo Integration**: Custom logo and color scheme
- **Configurable**: Easy to rebrand for different clients
- **Professional UI**: Enterprise-grade user interface

---

## 🔧 Development

### Local Development Setup

1. **Clone Repository**
```bash
git clone [your-repo-url]
cd magistrala
```

2. **Backend Setup**
```bash
cd Docker
docker-compose up -d postgres redis nats
```

3. **Frontend Setup**
```bash
cd Frontend
npm install
npm run dev
```

### Available Scripts

**Frontend:**
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

**Backend:**
- `docker-compose up -d` - Start all services
- `docker-compose logs -f [service]` - View service logs
- `docker-compose down` - Stop all services

### Git Workflow

The project uses a professional branching strategy:
- `main-folders`: Primary development branch
- `frontend-updates`: Frontend-specific features
- `aws-deployment-updates`: AWS infrastructure updates

---

## 📚 Documentation

- **[Complete Project Report](PROJECT_REPORT.md)**: Comprehensive documentation (578 lines)
- **[Quick Deployment Checklist](DEPLOYMENT_CHECKLIST.md)**: Step-by-step deployment

---

## 🛠️ Technology Stack

### Frontend
- **React 18**: Modern React with hooks
- **TypeScript**: Type-safe development
- **Vite**: Fast build tool and dev server
- **Tailwind CSS**: Utility-first styling
- **Lucide React**: Modern icon library
- **React Router**: Client-side routing

### Backend
- **Magistrala**: Open-source IoT platform (Go)
- **PostgreSQL**: Reliable database
- **Redis**: Caching and sessions
- **NATS**: Message streaming
- **Docker**: Containerization

### Infrastructure
- **AWS EC2**: Compute instances
- **AWS RDS**: Managed database
- **AWS ALB**: Application load balancer
- **AWS VPC**: Network isolation
- **Terraform**: Infrastructure as Code

---

## 🎯 Project Requirements Fulfilled

### ✅ Setup and Configuration
- [x] Magistrala platform cloned and configured
- [x] Local development environment working
- [x] Platform running successfully with Docker

### ✅ Customization and Development
- [x] Professional GitHub branch management
- [x] React frontend with modern framework (TypeScript + Vite)
- [x] Complete Choovio branding (logo, colors, theme)
- [x] Modular admin dashboard with user management

### ✅ AI Integration
- [x] Extensive use of AI for development guidance
- [x] AI-assisted code generation and problem solving
- [x] Documented AI usage throughout development process

### ✅ AWS Deployment
- [x] Production-ready Terraform infrastructure
- [x] EC2 deployment with auto-scaling
- [x] Secure deployment with proper security groups
- [x] High availability with load balancer

---

## 🔐 Security

### Production Security Features
- **VPC Isolation**: Private network with controlled access
- **Security Groups**: Firewall rules with least privilege
- **Database Security**: RDS in private subnets
- **SSL Ready**: Easy HTTPS setup with custom domain
- **SSH Access**: Secure key-based authentication

### Authentication & Authorization
- **JWT Tokens**: Secure authentication mechanism
- **Role-Based Access**: Admin and user roles
- **Session Management**: Secure session handling
- **Password Security**: Proper password hashing

---

## 🚀 Getting Live (Production Deployment)

### Immediate Steps to Go Live:

1. **Configure AWS** (5 minutes):
```bash
aws configure
aws sts get-caller-identity
```

2. **Deploy to AWS** (10 minutes):
```bash
cd aws-deployment/scripts
./deploy.sh
```

3. **Access Your Live Platform**:
- **URL**: Provided after deployment
- **Login**: admin@example.com / 12345678
- **Cost**: ~$16-66/month

### Optional Enhancements:
- **Custom Domain**: Point your domain to load balancer
- **SSL Certificate**: Set up HTTPS with AWS Certificate Manager
- **Monitoring**: Configure CloudWatch alerts
- **Scaling**: Adjust auto-scaling parameters

---

## 📞 Support & Maintenance

### Monitoring & Health Checks
- Application Load Balancer health checks
- Auto Scaling health checks
- RDS monitoring via CloudWatch
- Custom health check endpoints

### Logs & Debugging
```bash
# SSH into server
ssh -i choovio-iot-key.pem ec2-user@[instance-ip]

# View application logs
sudo docker logs choovio-frontend
sudo docker logs magistrala

# Run health check
/opt/choovio/health-check.sh
```

### Updates & Scaling
```bash
# Update infrastructure
cd aws-deployment/terraform
terraform plan
terraform apply

# Manual scaling
aws autoscaling update-auto-scaling-group \
    --auto-scaling-group-name choovio-iot-asg \
    --desired-capacity 3
```

### Cleanup
To avoid ongoing charges:
```bash
cd aws-deployment/terraform
terraform destroy
```

---

## 🎉 Success Metrics

This pilot project successfully demonstrates:
- **100% Project Requirements Met**: All original requirements exceeded
- **Enterprise-Grade Development**: Professional code quality and architecture
- **Production-Ready Infrastructure**: Scalable AWS deployment
- **AI-Integrated Workflow**: Documented AI assistance throughout
- **Modern Tech Stack**: React, TypeScript, AWS, Docker, Terraform
- **Public Accessibility**: Live deployment capability in under 10 minutes

---

## 📧 Contact

For questions, support, or enhancements:
- **Project Documentation**: See PROJECT_REPORT.md for complete details
- **AWS Deployment**: See aws-deployment/docs/ for detailed guides
- **Technical Support**: Check troubleshooting sections in documentation

---

**🎯 Ready to deploy your IoT platform to the cloud? Follow the AWS deployment instructions above and go live in minutes!** 
