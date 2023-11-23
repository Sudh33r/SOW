# Scope Document: GitHub Migration and Tool Integration

## 1. Introduction

This document outlines the detailed scope for migrating various Source Code Management (SCM) tools, Package Management Artifacts, Code Quality tools, and Security tools to GitHub. The migration includes detailed steps and strategies for each tool to ensure a smooth transition with minimal downtime and no data loss.

## 2. Source Code Management (SCM) Tools Migration

### 2.1 Bitbucket

#### Repositories with LFS and > 10GB
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Migrate Jenkins Pipelines to GitHub Actions.

### 2.2 Starteam

#### 2 Instances of StarTeam – 61 Repos/Views
- Integrate with Salesforce for Intake of Customer Issues.
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Define migration strategy ensuring minimal downtime and no data loss.
- Migrate Jenkins Pipelines to GitHub Actions.

### 2.3 SVN

#### 4 Instances of SVN
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Define migration strategy ensuring minimal downtime and no data loss.
- Migrate Jenkins Pipelines to GitHub Actions.

### 2.4 Perforce

#### 2 Instances of Perforce
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Define migration strategy ensuring minimal downtime and no data loss.
- Migrate Jenkins or Azure DevOps Pipelines to GitHub Actions.

### 2.5 TFS [60 Projects]

#### 2 Instances of TFS
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Define migration strategy ensuring minimal downtime and no data loss.
- Migrate Pipelines to GitHub Actions.

### 2.6 Azure DevOps

#### 45 Organizations
- Migrate Users, Permissions, LFS objects, Commits, Tags, Releases, Change Sets, History, Issues, Pull Requests, and Artifacts.
- Define migration strategy ensuring minimal downtime and no data loss.
- Migrate Pipelines to GitHub Actions.

## 3. Package Management Artifacts Migration

### 3.1 Nexus

- Centralize package management within GitHub Packages - Nexus migration.
- Migrate Nexus Artifacts to GitHub Packages.
- Update Nexus Artifacts to point to GitHub Packages in pipelines.

## 4. Code Quality

### 4.1 Sonarqube

- Standardize application Code Quality and code smell scanning using GitHub Advanced Security (GHAS).
- Document finalized architecture and procedure for admins and end users.
- Migrate from Sonarqube to GitHub Enterprise Cloud (GHEC) with rules.
- Design and implement GHAS Code Quality posture and reusable components.
- Define and implement Quality gates for pipelines.

## 5. Security Tools

### 5.1 Checkmarx [SAST]

- Design and implement GHAS security posture.
- Strategy and implementation document for transitioning from Checkmarx to GHAS.
- Migrate and Adoption plan for GHAS.
- Implementation for incremental versus comprehensive scanning.
- Process document for deduplicating vulnerabilities in GHAS.
- Process document for tracking vulnerabilities post-migration.
- Process document for managing security vulnerabilities during releases with GHAS.
- Identify, describe, and implement reporting capabilities for vulnerabilities in GHAS.
- Transition plan for applications generating reports for Customers.
- Blueprint for initiating GHAS scans prior to Jenkins/ADO builds.
- Define and implement Quality gates for pipelines.

### 5.2 Arnica [SCA]

- Design and implement GHAS security posture.
- Strategy and implementation document for transitioning from Arnica to GHAS.
- Adoption plan for GHAS.
- Implementation for incremental versus comprehensive scanning.
- Migrate Arnica to GHAS.
- Identify, describe, and implement reporting capabilities for vulnerabilities in GHAS.
- Process document for tracking vulnerabilities post-migration.
- Transition plan for applications generating reports for Customers.
- Blueprint for initiating GHAS scans prior to Jenkins/ADO builds.
- Define and implement Quality gates for pipelines.

## 6. Conclusion

This scope document provides a comprehensive plan for migrating various tools to GitHub, ensuring a seamless transition with enhanced features provided by GitHub Actions and Advanced Security. The outlined strategies prioritize minimal downtime and no data loss while improving overall efficiency and security in the development process.
