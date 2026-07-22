🚧 **Work in Progress**

# AI System Lifecycle

First, what is an AI system?
- An AI system is a computer system that uses data and AI models to perform tasks, make predictions or support decision-making. It also includes the people, processes, and technology needed to develop, operate, monitor and govern it.

## Overview

This artifact documents the complete lifecycle of an AI system, from inception to retirement. Organizations need to understand AI systems as managed assets with risks, controls and decision gates at every stage. 

AI systems don't exist in a vacuum. Like any software or hardware system, they are born, they mature, they degrade and eventually they are retired. Each stage has its own governance requirements, risks and decision points. Understanding this lifecycle is how we move from "AI is magic" to "AI is a managed asset". 

### The So What? 

Understanding this lifecycle enables organizations to oversee AI systems as managed assets throughtout their lifecycle with clearly defined ownership, controls, appropriate oversight, accountability and informed decision-making from inception through retirement. 

## The Seven Stages of AI System Lifecycle

### Stage 1: Foundation - What problem are we trying to solve?

Before we build or design anything, we need to understand:

- What is the business problem?
- How does AI help?
- Should AI be used at all?
- What would success look like?
- What could go wrong?

This is not technical. This is about clarity. 

A governance professional's job starts here. Organizations need to understand what problem the AI system is supposed to solve because they will later verify that it actually did, and that it didn't create new problems in the process. 

Example:
A bank is losing money to fraud and decides to build an AI system to automatically catch fraudulent attempts and stop them. 

Currently, a team of fraud analysts look at 100 transactions per day and flag the suspicious ones. They have learned over years what "suspicious" looks like, i.e., 

- Transactions at 3 AM from countries the customer never visits
- Amounts that are 10x higher than usual
- Multiple attempts in quick succession

Now imagine capturing the analysts' 10 years of decision patterns and teaching a machine to do this automatically. That machine becomes an AI system for fraud detection. 

#### Key Outputs

At the end of this stage, the organization should have:

✓ Clearly defined business problem

✓ Agreement on weather AI is appropriate to address the problem

✓ Success criteria

✓ Initial risks identified

✓ Executive approval to proceed

#### What should exist before we move to the next stage?

> An approved business case.

### Stage 2: Data - What information does the AI system need to learn?

Every AI system is only as good as the data it learns from. Before an AI system can make predictions or support decisions, it must first be provided with data that accurately represents the problem it is trying to solve.

Think of an AI system as a new employee on their first day. It has no understanding of the business problem it has been asked to solve. It learns by identifying patterns in the examples it is given. If those examples are incomplete, inaccurate or biased, the decisions it makes are likely to reflect the same weaknesses.

From a governance perspective, this is one of the most critical stages in the lifecycle. Poor-quality data can lead to poor-quality outcomes. Decisions made during this stage influence the accuracy, fairness, security and reliability of the AI system throughout its lifecycle.

There are **three** critical phases in this journey - 

#### i. Data Collection: Gather the data needed to train or support the AI system from relevant and reliable sources. 

The organization should ask:

- Where did this data come from?
- Do we have permission to use it?
- Is customer data being handled appropriately?
- Who owns the data?

#### ii. Data Preparation: Clean, organize, label and transform the data so it is suitable for use by the AI system.

The organization should ask:

- Has the data been cleaned consistently?
- Were any records removed? If yes, why?
- Is sensitive information protected?
- Is there documentation showing how the data was prepared?

#### iii. Data Validation: Verify the data to ensure it is suitable before using it to develop the AI system.

The organization should ask:

- Can this data be trusted?
- Is it representative of the real world?
- Has the data quality been formally reviewed?
- Has someone formally approved the dataset for use? 

Example:
An email provider wants to reduce the number of spam emails reaching users' inboxes and decides to build an AI system to automatically identify spam.

First, the organization _collects_ thousands of historical emails that have already been classified as either Spam or Not Spam. It then _prepares_ the data by removing duplicate emails, correcting inconsistencies and ensuring each email is labelled accurately. Finally, before the data is used to develop the AI system, it is _validated_ to confirm that it is accurate and approved for use. 

Only after completing these three phases is the dataset considered ready for model development. 

#### Key Outputs

At the end of this stage, the organization should have:

✓ Data collected from approved sources

✓ Data prepared and documented

✓ Data quality validated

✓ Privacy and security requirements addressed

✓ Approved dataset ready for model deployment

#### What should exist before we move to the next stage?

> An approved and validated dataset.

### Stage 3: Model Development - How is the AI system developed?

Now that we understand what information the AI system learns from, let's look at how that information is used to develop an AI model that can recognize patterns and make predictions.

To start, imagine a real estate company wants to estimate the selling price of houses based on factors such as location, size, age and number of bedrooms. During model development, the AI system is provided with thousands of historical property records where the selling prices are already known. By analysing these examples, it learns the relationship between a property's characteristics and its selling price. Once the learning process is complete, the model can estimate the selling price of a new house it has never seen before based on the patterns it has identified. 

It is important to remember - **The model is learning patterns, not memorising answers.**

There are **three** key concepts to understand:

#### i. The model is a pattern extraction engine
- A trained AI model is essentially a compressed representation of patterns in your training data.
- Example: A house near the city centre with similar characteristics to previously sold homes is likely to have a similar market value.

#### ii. The model can learn the wrong thing
- A model can learn patterns that don't actually generalize. This is called overfitting i.e. the model learned patterns specific to the training data that don't apply to the real world.
- Example: The model predicts that every expensive house has a swimming pool simply because most houses in the training data happened to have one.

#### iii. The model needs validation before it is trusted
- Organizations need to ask, _does the AI model actually work on data it's never seen before?_
- Example: The model performs well during training but struggles to accurately estimate the prices of newly listed houses.

As governance professionals, we don't necessarily need to understand the mathematics behind neural networks. However, we do need to ask the right questions to determine whether an AI model is reliable, explainable and suitable for its intended use.

#### **Question 1:** Is the model generalizing or overfitting? 
- What's the performance on training data vs unseen test data?
- Are the performance results similar or significantly different?
**Governance Risk:** If the model only works on training data, it is unlikely to perform reliably in production.

#### **Question 2:** Can we explain what the model learned?
- What patterns does the model use to make decisions?
- Can these decisions be understood and explained to stakeholders?
**Governance Risk:** Poor explainability makes it difficult to audit the model, identify bias, investigate incidents or justify decisions to regulators, customers or courts.

#### **Question 3:** What are the model's failure modes?
- Under what conditions does the model make mistakes?
- Are the limitations understood and documented?
**Governance Risk:** A model may appear highly accurate overall while performing poorly for specific scenarios, user groups or types of data. Its important to understand these limitations before deploying the model.

#### Key Outputs

At the end of this stage, the organization should have:

✓ A trained AI model

✓ Model performance evaluated on training and unseen test data

✓ Model limitations and failure modes identified and documented

✓ Evidence that the model is suitable for its intended purpose

✓ Model approved to proceed for validation and testing

#### What should exist before we move to the next stage?

> A trained and evaluated AI model that is ready for formal validation and testing.



