import React from "react";
import { FaGithub, FaLinkedin, FaEnvelope } from "react-icons/fa";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

const Home = () => {
  return (
    <div className="container mx-auto p-6">
      <header className="text-center">
        <h1 className="text-4xl font-bold">Jonas Henri Cobbah</h1>
        <p className="text-lg text-gray-600 mt-2">
          🚀 Cloud & DevOps Engineer | Site Reliability Engineer (SRE) | Infrastructure Automation
        </p>
      </header>

      <section className="mt-8">
        <h2 className="text-2xl font-semibold">🔧 Technical Expertise</h2>
        <ul className="grid grid-cols-2 md:grid-cols-3 gap-4 mt-4 text-gray-700">
          <li><strong>Cloud & Infrastructure:</strong> AWS | Azure | GCP | OpenStack</li>
          <li><strong>Infrastructure as Code:</strong> Terraform | CloudFormation | AWS CDK | Ansible | Packer</li>
          <li><strong>Containerization & Orchestration:</strong> Docker | Kubernetes (EKS, AKS, GKE) | Helm | ArgoCD | Istio</li>
          <li><strong>CI/CD & Automation:</strong> GitHub Actions | GitLab CI | Jenkins | Spinnaker | AWS CodePipeline</li>
          <li><strong>Monitoring & Observability:</strong> Prometheus | Grafana | CloudWatch | Datadog | ELK Stack</li>
          <li><strong>Security & Compliance:</strong> AWS IAM | Vault | CIS Benchmarks | PCI-DSS | ISO 27001</li>
          <li><strong>Programming & Scripting:</strong> Python | Bash | Go | PowerShell</li>
          <li><strong>Databases & Storage:</strong> PostgreSQL | MySQL | DynamoDB | MongoDB</li>
          <li><strong>Networking & Traffic Management:</strong> NGINX | ALB | NLB | Route 53 | Cloud DNS</li>
        </ul>
      </section>

      <section className="mt-8">
        <h2 className="text-2xl font-semibold">📌 What I Do</h2>
        <ul className="list-disc pl-6 mt-4 text-gray-700">
          <li>✅ Cloud Infrastructure Design & Automation with Terraform, Ansible, and Kubernetes.</li>
          <li>✅ CI/CD Pipeline Optimization using Jenkins, GitHub Actions, and GitLab CI/CD.</li>
          <li>✅ Site Reliability & Performance Engineering with SLOs, SLIs, and automated incident response.</li>
          <li>✅ DevSecOps & Compliance with IAM policies and security best practices.</li>
          <li>✅ Monitoring & Logging using Prometheus, ELK, and Datadog.</li>
        </ul>
      </section>

      <section className="mt-8">
        <h2 className="text-2xl font-semibold">📂 Featured Projects</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 mt-4">
          <Card>
            <CardContent>
              <h3 className="text-xl font-semibold">AWS Terraform Modules</h3>
              <p className="text-gray-600">A collection of Terraform modules for AWS infrastructure automation.</p>
              <a href="https://github.com/abeiku12/aws-eks-terraform/tree/master" className="text-blue-500">View Project</a>
            </CardContent>
          </Card>
          <Card>
            <CardContent>
              <h3 className="text-xl font-semibold">Kubernetes Helm Charts</h3>
              <p className="text-gray-600">Production-ready Helm charts for deploying cloud-native applications.</p>
              <a href="https://github.com/abeiku12/helm" className="text-blue-500">View Project</a>
            </CardContent>
          </Card>
          <Card>
            <CardContent>
              <h3 className="text-xl font-semibold">CI/CD Pipeline Automation</h3>
              <p className="text-gray-600">Automated CI/CD workflows using GitHub Actions and Jenkins.</p>
              <a href="https://github.com/abeiku12/maven-web-application" className="text-blue-500">View Project</a>
            </CardContent>
          </Card>
        </div>
      </section>

      <section className="mt-8">
        <h2 className="text-2xl font-semibold">📫 Let's Connect</h2>
        <div className="flex gap-4 mt-4">
          <Button asChild>
            <a href="https://www.linkedin.com/in/jonas-cobbah-722879335" target="_blank" rel="noopener noreferrer">
              <FaLinkedin className="mr-2" /> LinkedIn
            </a>
          </Button>
          <Button asChild>
            <a href="https://github.com/abeiku12" target="_blank" rel="noopener noreferrer">
              <FaGithub className="mr-2" /> GitHub
            </a>
          </Button>
          <Button asChild>
            <a href="mailto:cobbahh@gmail.com">
              <FaEnvelope className="mr-2" /> Email
            </a>
          </Button>
        </div>
      </section>
    </div>
  );
};

export default Home;
