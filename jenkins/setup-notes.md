## Jenkins Setup Notes
- **OS:** Amazon Linux 2023
- **Java Version:** `java-17-amazon-corretto`
- **Jenkins Version:** Jenkins 2.492.3
- **Installation Steps:**
  - Installed Java 17 using Corretto
  - Installed Jenkins via official repo
  - Enabled and started Jenkins service
  - Accessed via public IP on port 8080
	```bash
	sudo dnf update -y
	sudo dnf install java-17-amazon-corretto -y
	sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
	sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
	sudo dnf install jenkins -y
	sudo systemctl enable jenkins
	sudo systemctl start jenkins
	sudo dnf install docker git -y
	sudo systemctl start docker
	sudo systemctl enable docker
	sudo usermod -aG docker jenkins
	```