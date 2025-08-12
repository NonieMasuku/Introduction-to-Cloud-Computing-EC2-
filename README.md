# Introduction-to-Cloud-Computing-EC2
## **1. What is Amazon EC2?**

Amazon EC2 (Elastic Compute Cloud) is **AWS’s virtual server service**.
It lets you run applications on AWS infrastructure without buying physical servers. You choose:

* **Instance type** (CPU, memory, network capacity)
* **Operating system** (Linux, Windows, etc.)
* **Region** where it runs
* **Scaling** up/down as needed

💡 **Key point:** Think of it as renting a flexible, resizable server in the cloud that you pay for based on how much you use.

## **2. AWS Shared Responsibility Model (specific to EC2)**

> AWS works on a **shared responsibility model**, meaning **AWS handles the “cloud infrastructure”** while **you handle what you put inside it**.

**AWS is responsible for:**

* Physical security of data centers
* Networking infrastructure
* Virtualization layer (the hypervisor that runs EC2)
* Hardware maintenance

**You are responsible for:**

* Your EC2 instance’s OS updates & patches
* Application security & configurations
* Managing firewalls/security groups
* Data encryption (unless using managed AWS encryption)
* IAM user access control

💡 Example: AWS keeps the server hardware safe from intruders, but if you leave your EC2 instance with a weak password, that’s on you.

## **3. EC2 Pricing Models**

AWS offers different **payment options** depending on how you plan to use EC2:

| **Model**         | **Best for**                                     | **How you pay**                               |
| ----------------- | ------------------------------------------------ | --------------------------------------------- |
| **On-Demand**     | Short-term, unpredictable workloads              | Pay per second/hour — stop anytime            |
| **Reserved**      | Steady workloads for 1–3 years                   | Commit to term for a big discount (up to 72%) |
| **Spot**          | Flexible workloads that can handle interruptions | Bid for unused capacity (up to 90% off)       |
| **Savings Plans** | Flexible commitment across EC2 & other services  | Commit to \$/hr usage for 1–3 years           |
| **Free Tier**     | Learning/testing                                 | 750 hrs/month of t2.micro for 12 months       |

💡 **Tip:** For a new AWS learner, the **Free Tier** + **Spot Instances** for testing can save a lot of money.

## **4. Key EC2 Concepts You Should Know**

* **AMI (Amazon Machine Image):** A template to launch instances with OS + pre-installed software.
* **Instance Types:** Families like `t2.micro` (small, general-purpose) or `c5.large` (compute-optimized).
* **Security Groups:** Virtual firewalls controlling inbound & outbound traffic.
* **EBS (Elastic Block Store):** Persistent disk storage for EC2.
* **Elastic IP:** Static public IP address for your instance.
* **Auto Scaling:** Automatically adjusts instance count based on traffic.

## **5. Example Use Cases**

* Running a web app backend
* Hosting databases (though RDS is usually better)
* Machine learning workloads
* Batch data processing
* Game servers


![Amazon EC2](https://github.com/user-attachments/assets/76f4195e-2d35-4e25-a6c5-d5e3ddfe2e6d)

