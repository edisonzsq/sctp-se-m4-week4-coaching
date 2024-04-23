# Coaching | SCTP in SE | Module 4 | DevOps Week 4

<details>
<summary> 1. Next.js and Vercel </summary>

This guide will take you through the process of setting up a Next.js project, pushing it to GitHub, and configuring automatic deployments to Vercel. Each new push to GitHub will trigger a Vercel deployment, creating a dedicated URL for that deployment.

## Prerequisites

Before you begin, ensure you have the following:
- Node.js installed (LTS version recommended).
- Git installed and configured.
- A GitHub account.
- A Vercel account.

## Step 1: Initialize a Next.js Project

1. Open your terminal.
2. Create a new Next.js app by running:
```bash
   npx create-next-app@latest my-next-project
```
3. Change into project directory:
```bash
cd my-next-project
```

## Step 2: Create a Repository on GitHub

1. Go to GitHub and log in to your account.
1. Click on the "New" button to create a new repository.
1. Name your repository and leave it public for easier access.
1. Do not initialize it with a README, .gitignore, or license.

## Step 4: Push Your Local Repository to GitHub

1. Copy the remote repository URL from GitHub.
2. Link your local repository with the remote repository:
```bash
git remote add origin <YOUR_GITHUB_REPO_URL>
```
3. Push your changes to GitHub:
```bash
git push -u origin master
```

## Step 5: Step 5: Connect Your GitHub Repository to Vercel

1. Log in to your Vercel account.
1. Click on "New Project".
1. Select your GitHub repository.
1. Click on "Import" and follow the setup instructions, keeping most settings at their defaults.

## Step 6: Automatic Deployment Setup

1. Every push to your GitHub repository will now trigger a new deployment to Vercel.
1. Vercel automatically creates a unique URL for each deployment.

## Step 7: Viewing Deployment History

1. Go to your project's dashboard on Vercel.
1. Click on the "Deployments" tab to view all the deployments.
1. Each entry shows the deployment's unique URL.

## Conclusion

You now have a fully functional workflow that initializes a Next.js project, tracks it with Git, and deploys updates to Vercel with unique URLs for each push. This setup is ideal for continuous integration and delivery practices in modern web development.

</details>

<details>
<summary> 2. Understanding Other Roles - SRE and Platform Engineering </summary>

## Definitions

**DevOps** is a set of practices and philosophies aimed at shortening the development life cycle, ensuring continuous delivery with high software quality. It emphasizes collaboration between development and operations teams.

**Platform Engineering** involves creating and maintaining shared platforms used by development teams to run their applications. It focuses on building and scaling infrastructure and tooling to enhance developer productivity and operational efficiency.

**Site Reliability Engineering (SRE)** is a discipline that incorporates aspects of software engineering and applies them to infrastructure and operations problems. The goal is to create scalable and highly reliable software systems.

## Comparison Table

| Aspect               | DevOps                                       | Platform Engineering                             | SRE                                            |
|----------------------|----------------------------------------------|--------------------------------------------------|------------------------------------------------|
| **Focus**            | Collaboration between dev and ops            | Building and scaling shared platforms            | Operational reliability of software            |
| **Goal**             | Improve deployment frequency, error recovery | Enhance developer productivity, efficiency       | Achieve high system reliability and uptime     |
| **Primary Tasks**    | CI/CD pipelines, monitoring, automation      | Building internal tools, infrastructure upkeep   | Incident management, post-mortem analysis      |
| **Outcome**          | Faster time to market, fewer failures        | Streamlined workflows, consistent environments   | Predictable, reliable system behavior          |

## Pictorial Comparison

<img src="https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fa0fdc1b7-dde6-4afb-b462-713c1bd016e9_800x1146.jpeg" />

</details>