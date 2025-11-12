---
title: "Understanding Your JobRunr Pro Business License"
description: "A clear explanation of our 'per project' licensing model for production environments."
date: 2025-11-12
---

We want our licensing to be simple and fair. You may have seen our license is for **one production project**. We get questions on what this means in practice.

This page explains exactly what one "project" is and what your license covers.

The short answer is: **A Pro Business license covers one logical application in production.**

A **JobRunr Pro Enterprise license** on the other hand is truly **unlimited**. 
You can use it in as many projects as you want. 

## What is a "Project"?

A "project" is a single, logical business application or system. It is defined by its own distinct namespace and purpose.

For example:

* A **"Payments System"** (like `org.jobrunr.payments`) is **one project**.
* A **"CRM System"** (like `org.jobrunr.crm`) is a **second project**.

Even if they are developed by the same company, these are two different projects with different business logic. Each would require its own [JobRunr Pro Business license]({{< ref "/pro.md" >}}) for its production environment.

## What Your License Includes

Your single project license includes:

* **Unlimited Non-Production Environments**
    You can use your license key in all development, testing, QA, and staging environments for free. We only license your single production environment.

* **Unlimited Developers**
    We do not charge per seat. Your whole team is covered.

* **Unlimited Servers, Nodes, or Pods**
    We do not care how many instances you run for your project. You can scale your application to hundreds of servers. It is still one project.

## Common Scenarios

Here are a few examples to make it even clearer.

### Scenario 1: The Hybrid Cloud / Distributed Scenario

* **Your Setup:** You run one logical application. Your base servers are on-premise. When demand is high, you scale up by adding more worker servers in the cloud (AWS, Azure, etc.).
* **Your License:** You need **one license**. This is all considered one production project, regardless of where the servers are physically located. We do not charge for extra nodes.

### Scenario 2: Multiple Environments

* **Your Setup:** You have a development environment, a staging environment, and a production environment for your "Payments System".
* **Your License:** You need **one license**. We only charge for the production environment.

### Scenario 3: Separate Products

* **Your Setup:** You have two completely separate products.
    1.  An **"E-commerce Platform"** (e.g., `org.jobrunr.ecommerce`).
    2.  An **"Internal HR Tool"** (e.g., `org.jobrunr.hr`).
* **Your License:** You need **two licenses**. These are two different logical projects, serving different business purposes.

### Final Scenario: The Microservice Architecture

* **Your Setup:** You have a large application built with multiple microservices. For example, a `payment-service`, a `fraud-detector`, and a `notification-service`.
* **The Challenge:** Because each microservice is its own application, they would technically each be a separate "project". This would mean needing a separate license for every service, which is not ideal.
* **Our Solution:** We understand this. For this exact situation, we offer a specific **Pro Business package for microservices**. This package provides a cost-effective way to license all the microservices that are part of one larger logical application.
* **Your License:** If you are building with microservices, contact us about the **Pro Business microservice package** for a quote that fits your architecture.

### How Does This Relate to the Database?

A single project (like your "Payments System" and all its microservices) will typically use one shared JobRunr database.

Two different projects (like "Payments" and "CRM") will almost always use two **separate** JobRunr databases.

While the database is not the *definition* of a project, it's a good guideline. The definition is about the **logical application**. Our licensing is based on this fair-use principle.

## Still Unsure?

Our goal is fair and simple pricing. We are not trying to trick you.

If you have a complex setup or just want to double-check if your setup counts as one or more projects, please [contact us]({{< ref "/contact.md" >}}). We are happy to help.