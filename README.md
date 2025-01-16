# Complete AI Guide

# Prompt engineering guide


## Contents
- [Understanding Prompt Engineering](#understanding-prompt-engineering)
- [The Anatomy of an Effective Prompt](#the-anatomy-of-an-effective-prompt)
- [Template: Creating Customized Learning Paths](#template-creating-customized-learning-paths)
- [Real-World Example](#real-world-example)
- [Advanced Prompt Engineering Techniques](#advanced-prompt-engineering-techniques)
- [Common Pitfalls to Avoid](#common-pitfalls-to-avoid)
- [Best Practices for Prompt Engineering](#best-practices-for-prompt-engineering)
- [Conclusion](#conclusion)
- [Beginner Prompts](#beginner-prompts)
  - [User Authentication System](#1-user-authentication-system)
  - [Basic To-Do App](#2-basic-to-do-app)
  - [Simple Blog](#3-simple-blog)
- [Intermediate Prompts](#intermediate-prompts)
  - [Sports Community App](#1-sports-community-app)
  - [E-commerce Shopping Cart](#2-e-commerce-shopping-cart)
  - [Recipe Manager for Restaurants](#3-recipe-manager-for-restaurants)
- [Advanced Prompts](#advanced-prompts)
  - [Collaborative Task Manager](#1-collaborative-task-manager)
  - [Social Media App for Athletes](#2-social-media-app-for-athletes)
  - [Restaurant Analytics Dashboard](#3-restaurant-analytics-dashboard)
  - [E-commerce Recommendation System](#4-e-commerce-recommendation-system)
- [Additional Project Ideas](#additional-project-ideas)
- [Why These Prompts Are Valuable](#why-these-prompts-are-valuable)
- [Project Overview](#project-overview)
- [Core Features Implementation](#core-features-implementation)
  - [Authentication Flow](#1-authentication-flow)
  - [Chat Implementation](#2-chat-implementation)
  - [OpenAI Integration](#3-openai-integration)
  - [Credits System](#4-credits-system)
  - [Stripe Integration](#5-stripe-integration)
- [Database Schema](#database-schema)
- [User Interface Components](#user-interface-components)
  - [Profile Section](#profile-section)
  - [Credits Purchase UI](#credits-purchase-ui)
- [Best Practices & Tips](#best-practices--tips)
- [Common Issues & Solutions](#common-issues--solutions)
- [Technical Stack](#technical-stack)
- [Development Environment Setup](#development-environment-setup)
- [Advanced Features](#advanced-features)
  - [Rate Limiting](#rate-limiting)
  - [Analytics Integration](#analytics-integration)
  - [Prompt Management](#prompt-management)
- [Testing Strategy](#testing-strategy)
- [Deployment Guide](#deployment-guide)

## Understanding Prompt Engineering

Prompt engineering is the art and science of crafting effective inputs for AI language models like ChatGPT. It involves understanding both the capabilities and limitations of AI models to generate optimal responses. Success in prompt engineering requires:

- **Technical Understanding**: Knowledge of how LLMs process and interpret text
- **Clear Communication**: Ability to articulate requirements precisely
- **Iterative Refinement**: Willingness to test and improve prompts
- **Context Awareness**: Understanding of the model's training boundaries

## The Anatomy of an Effective Prompt

A well-structured prompt typically includes several key components:

1. **Context Setting**: 
   - Define the AI's role (e.g., "Act as a senior software architect")
   - Establish expertise level (e.g., "Explain this as if to a junior developer")
   - Set the scope (e.g., "Focus on Python best practices")

2. **Input Parameters**:
   - User background information
   - Specific use case details
   - Relevant constraints
   - Technical requirements

3. **Clear Instructions**:
   - Step-by-step task breakdown
   - Priority ordering
   - Dependencies between tasks
   - Expected deliverables

4. **Output Format**:
   - Response structure (e.g., bullet points, numbered lists)
   - Required sections
   - Formatting preferences
   - Length constraints

## Template: Creating Customized Learning Paths

Here's a powerful prompt template for generating personalized learning experiences:

### User Profile Section
- Age
- Education Level
- Occupation
- Field of Interest
- Preferred Learning Style
- Current Understanding Level
- Key Goals
- Available Learning Time

### Enhanced Task Instructions
1. Break down the main topic into structured subtopics
   - Create logical progression
   - Identify prerequisites
   - Set milestone markers
   - Include knowledge checkpoints

2. Provide summaries for each section
   - Key concepts overview
   - Common pitfalls
   - Best practices
   - Real-world applications

3. Suggest relevant resources
   - Official documentation
   - Tutorial links
   - Practice exercises
   - Community forums

4. Maintain appropriate tone and engagement
   - Match user expertise level
   - Include motivational elements
   - Provide progress markers
   - Add interactive components

5. Create a weekly learning schedule
   - Time-boxed activities
   - Progress tracking
   - Review sessions
   - Practice assignments

## Real-World Example

Let's look at how this template works for a software engineer learning machine learning:

### Sample User Profile
- Age: 25
- Education: Undergraduate
- Occupation: Software Engineer
- Interest: Machine Learning
- Learning Style: Hands-on
- Level: Beginner
- Goal: Build basic ML models
- Time Available: 6 hours/week

### Enhanced Learning Path
1. **Introduction to Machine Learning** (Week 1-2)
   - Core concepts and definitions
     - Supervised vs unsupervised learning
     - Classification vs regression
     - Model training workflow
   - Types of ML approaches
     - Traditional algorithms
     - Neural networks
     - Deep learning basics
   - Practical exercises
     - Python basics for ML
     - NumPy and Pandas fundamentals
     - Basic data manipulation

2. **Core ML Concepts**
   - Dataset management
   - Feature engineering
   - Data preprocessing

3. **Basic Algorithms**
   - Linear regression
   - Decision trees
   - Hands-on implementation

4. **Evaluation Methods**
   - Key metrics
   - Testing approaches
   - Model validation

5. **Practical Application**
   - Real-world project
   - Implementation steps
   - Performance optimization

## Advanced Prompt Engineering Techniques

1. **Chain of Thought Prompting**
   - Break complex problems into steps
   - Show reasoning process
   - Include intermediate calculations
   - Validate each step

2. **Few-Shot Learning**
   - Provide example pairs
   - Demonstrate patterns
   - Include edge cases
   - Show error handling

3. **Role-Based Prompting**
   - Define expertise level
   - Set communication style
   - Establish authority
   - Maintain consistency

4. **Iterative Refinement**
   - Start with basic prompts
   - Analyze responses
   - Identify improvements
   - Refine systematically

## Common Pitfalls to Avoid

1. **Ambiguous Instructions**
   - Unclear objectives
   - Missing context
   - Vague requirements
   - Inconsistent formatting

2. **Information Overload**
   - Too many requirements
   - Excessive details
   - Complex structures
   - Conflicting instructions

## Best Practices for Prompt Engineering

1. Be specific and detailed
   ```example
   ❌ "Write code for a sorting algorithm"
   ✅ "Write a Python implementation of the quicksort algorithm with detailed comments explaining the partition logic and time complexity"
   ```

2. Use clear formatting
   ```example
   ❌ "give me info about react hooks explain lifecycle methods and include code examples"
   ✅ "Explain React hooks with:
      - Brief introduction to each hook
      - Code examples for useState and useEffect
      - Comparison with lifecycle methods
      - Common use cases
      Please format the response with markdown and include syntax-highlighted code blocks."
   ```

3. Break down complex requests
   ```example
   ❌ "Create a full-stack web application"
   ✅ "Let's build a web application in steps:
      1. First, design the database schema for a user authentication system
      2. Then, create the API endpoints for user registration and login
      3. Finally, implement the frontend login form
      Please provide the solution for step 1 first."
   ```

4. Include examples when needed
   ```example
   ❌ "Help me write regex for email validation"
   ✅ "Help me write a regex pattern for email validation. Here are some test cases it should handle:
      Valid: user@domain.com, user.name@domain.co.uk
      Invalid: user@domain, @domain.com, user@.com"
   ```

5. Specify output format preferences
   ```example
   ❌ "Explain Docker concepts"
   ✅ "Explain Docker concepts in a table format with three columns:
      | Concept | Description | Example Command |
      Include: containers, images, volumes, and networks"
   ```

## Conclusion

Effective prompt engineering is crucial for getting the most out of AI tools like ChatGPT. By following structured templates and understanding key components, you can create more effective prompts that generate better results.

# Build AI Projects fast

If you're looking to hone your software development skills and fast-track your growth into a highly proficient engineer, these project ideas will provide you with the right mix of foundational concepts, intermediate challenges, and advanced features. Here's how to structure your learning journey, divided into beginner, intermediate, and advanced levels.


## Table of Contents
- [Beginner Prompts](#beginner-prompts)
  - [User Authentication System](#1-user-authentication-system)
  - [Basic To-Do App](#2-basic-to-do-app)
  - [Simple Blog](#3-simple-blog)
- [Intermediate Prompts](#intermediate-prompts)
  - [Sports Community App](#1-sports-community-app)
  - [E-commerce Shopping Cart](#2-e-commerce-shopping-cart)
  - [Recipe Manager for Restaurants](#3-recipe-manager-for-restaurants)
- [Advanced Prompts](#advanced-prompts)
  - [Collaborative Task Manager](#1-collaborative-task-manager)
  - [Social Media App for Athletes](#2-social-media-app-for-athletes)
  - [Restaurant Analytics Dashboard](#3-restaurant-analytics-dashboard)
  - [E-commerce Recommendation System](#4-e-commerce-recommendation-system)
- [Additional Project Ideas](#additional-project-ideas)
- [Why These Prompts Are Valuable](#why-these-prompts-are-valuable)


---

## Beginner Prompts

### 1. User Authentication System  
**Objective:** Build a simple user authentication system using Supabase.  
**Features to Include:**  
- Email and password login functionality  
- User signup, login, and logout  
- Password reset functionality via email  

### 2. Basic To-Do App  
**Objective:** Create a full-stack to-do list application using React (frontend) and Firebase (backend).  
**Features to Include:**  
- Add, update, delete, and mark tasks as complete  
- Real-time database updates  
- User-friendly interface  

### 3. Simple Blog  
**Objective:** Develop a blog application for creating, editing, and deleting posts.  
**Tech Stack:**  
- Backend: Node.js with Express  
- Database: MongoDB  
- Frontend: HTML/CSS  

---

## Intermediate Prompts

### 1. Sports Community App  
**Objective:** Develop a sports community app using Supabase.  
**Features to Include:**  
- User roles: Manager, Coach, and Student  
- Role-based access control  
  - Managers can add team information  
  - Coaches can schedule practice sessions  
  - Students can view their schedules  

### 2. E-commerce Shopping Cart  
**Objective:** Build a shopping cart app using React, Node.js, Express, and MongoDB.  
**Features to Include:**  
- Product dashboard  
- Add items to cart, update quantities, and calculate total cost  
- Persist cart data using sessions or a database  

### 3. Recipe Manager for Restaurants  
**Objective:** Create a restaurant management app.  
**Features to Include:**  
- User and manager roles using Supabase authentication  
- Form for managers to add recipes  
- Customer interface to view recipes and add items to a shopping cart  
- Manager dashboard to view customer orders  

---

## Advanced Prompts

### 1. Collaborative Task Manager  
**Objective:** Build a task manager with real-time features.  
**Features to Include:**  
- Real-time updates using WebSockets  
- User roles: Admin, Manager, and Team Member  
- Supabase integration for real-time updates and user authentication  

### 2. Social Media App for Athletes  
**Objective:** Create a social media app for athletes using Next.js and Firebase.  
**Features to Include:**  
- User profiles, photo uploads, post likes, and comments  
- Infinite scrolling for posts  
- Real-time notifications using Firebase Cloud Messaging  

### 3. Restaurant Analytics Dashboard  
**Objective:** Extend the restaurant management app with advanced analytics.  
**Features to Include:**  
- Analytics for order trends, popular dishes, and revenue  
- Data visualization using Chart.js or D3.js  
- Real-time notifications for managers when new orders are placed  

### 4. E-commerce Recommendation System  
**Objective:** Enhance the e-commerce app with machine learning-powered recommendations.  
**Features to Include:**  
- Personalized product suggestions based on browsing and purchase history  
- Machine learning models hosted on AWS Lambda  

---

## Additional Project Ideas

- **Online Course Platform:** Allow instructors to upload courses, and students to enroll and take lessons. Include a discussion forum.  
- **Event Management System:** Create a platform where users can create and RSVP to events, with admin controls for event approvals.  
- **AI Chatbot Integration:** Add an AI chatbot to any app using OpenAI GPT APIs to assist users with queries.  

---

### Why These Prompts Are Valuable  
These projects will:  
- Teach you the core technologies in software development.  
- Help you integrate advanced features like authentication, real-time updates, and analytics.  
- Provide practical experience, preparing you for real-world challenges.  

## AI projects built with Claude

Image comparison tool
https://claude.site/artifacts/a49309c9-49ec-4888-a790-891894001525 

Rubics cube simulator
https://claude.site/artifacts/0a4a1e14-85d8-4169-b251-6ceebda740cb 

Bloom filter visualization
https://claude.site/artifacts/2e673219-d056-44b8-9642-b0bbee928c54 

Self playing snake game
https://claude.site/artifacts/5574c1eb-ea43-4e20-9d89-c96b9d4cf1de 

Reddit thread formatter
https://claude.site/artifacts/6892d6ff-5f2e-4731-bb52-14fd3ec781db 

Bitcoin game
https://claude.site/artifacts/cf93dea8-1b44-4c44-8ff3-a2eef2a7d8cd 

Music drum pad
https://claude.site/artifacts/091a4c98-f9fc-4601-ae3d-29e3382cd5a3 

TDEE, Macronutrient, and BMI Calculator
https://claude.site/artifacts/bab072fe-4873-4a5f-b626-a076341c2d76 

Stock Option Call Analyzer
https://claude.site/artifacts/cd452263-d93a-4506-94b6-6dcb9681512f 

Flappy bird game
https://x.com/NickADobos/status/1803837860635627558 

Sudoku solver
https://claude.site/artifacts/22a509b7-5f6a-478a-b56c-298898c3cba6 

Python interpreter
https://claude.site/artifacts/3fdd108a-4937-4ca6-b2f4-3cf370fec57c 

Drum synth pad
https://claude.site/artifacts/4a0693bb-db93-4e81-8342-fd0921ae49b5 

Diff checker
https://claude.site/artifacts/020cf820-7c4b-406b-aeb5-e876337cd6af 

Double pendulum simulator
https://claude.site/artifacts/33451efb-3ddd-496e-95f9-3cc08c6c72de 

By tackling these prompts, you'll progressively master the skills needed to become a 100x engineer.

# Building an AI SaaS

## Table of Contents
- [Project Overview](#project-overview)
- [Core Features Implementation](#core-features-implementation)
  - [Authentication Flow](#1-authentication-flow)
  - [Chat Implementation](#2-chat-implementation)
  - [OpenAI Integration](#3-openai-integration)
  - [Credits System](#4-credits-system)
  - [Stripe Integration](#5-stripe-integration)
- [Database Schema](#database-schema)
- [User Interface Components](#user-interface-components)
  - [Profile Section](#profile-section)
  - [Credits Purchase UI](#credits-purchase-ui)
- [Best Practices & Tips](#best-practices--tips)
- [Common Issues & Solutions](#common-issues--solutions)
- [Technical Stack](#technical-stack)
- [Development Environment Setup](#development-environment-setup)
- [Advanced Features](#advanced-features)
  - [Rate Limiting](#rate-limiting)
  - [Analytics Integration](#analytics-integration)
  - [Prompt Management](#prompt-management)
- [Testing Strategy](#testing-strategy)
- [Deployment Guide](#deployment-guide)

## Project Overview

We'll build an AI chat application with:
- Free tier (5 messages)
- Authentication
- Credits system
- Payment integration
- Chat history
- User profiles

## Core Features Implementation

### 1. Authentication Flow
```typescript
// src/contexts/AuthContext.tsx
import { createContext, useContext, useState } from 'react';
import { supabase } from '../lib/supabase';

export const AuthContext = createContext({});

export function AuthProvider({ children }) {
  const [user, setUser] = useState(null);
  const [session, setSession] = useState(null);

  // Check for free messages before requiring auth
  const checkAuthRequirement = async (messageCount) => {
    if (messageCount >= 5 && !session) {
      return true; // Require auth
    }
    return false;
  };

  return (
    <AuthContext.Provider value={{ user, session, checkAuthRequirement }}>
      {children}
    </AuthContext.Provider>
  );
}
```

### 2. Chat Implementation
```typescript
// src/components/Chat.tsx
import { useState, useEffect } from 'react';
import { supabase } from '../lib/supabase';
import { useAuth } from '../contexts/AuthContext';

export default function Chat() {
  const [messages, setMessages] = useState([]);
  const [messageCount, setMessageCount] = useState(0);
  const { session, checkAuthRequirement } = useAuth();

  const handleSendMessage = async (content) => {
    // Check free tier limit
    const requireAuth = await checkAuthRequirement(messageCount);
    if (requireAuth) {
      showAuthModal();
      return;
    }

    // Process message with OpenAI
    const response = await processWithAI(content);
    
    // Save to database if authenticated
    if (session) {
      await saveToDatabase(content, response);
    }
    
    setMessageCount(prev => prev + 1);
  };
}
```

### 3. OpenAI Integration
```typescript
// src/lib/openai.ts
import { Configuration, OpenAIApi } from 'openai';

const configuration = new Configuration({
  apiKey: process.env.OPENAI_API_KEY,
});

const openai = new OpenAIApi(configuration);

export async function processWithAI(content: string) {
  const completion = await openai.createChatCompletion({
    model: "gpt-3.5-turbo",
    messages: [{ role: "user", content }],
  });

  return completion.data.choices[0].message.content;
}
```

### 4. Credits System
```typescript
// src/lib/credits.ts
export async function checkCredits(userId: string) {
  const { data: credits } = await supabase
    .from('credits')
    .select('amount')
    .eq('user_id', userId)
    .single();

  return credits?.amount || 0;
}

export async function deductCredit(userId: string) {
  const { data, error } = await supabase
    .from('credits')
    .update({ amount: credits - 1 })
    .eq('user_id', userId);

  return !error;
}
```

### 5. Stripe Integration
```typescript
// src/lib/stripe.ts
import Stripe from 'stripe';

const stripe = new Stripe(process.env.STRIPE_SECRET_KEY);

export async function createCheckoutSession(userId: string, priceId: string) {
  const session = await stripe.checkout.sessions.create({
    line_items: [{
      price: priceId,
      quantity: 1,
    }],
    mode: 'payment',
    success_url: `${process.env.DOMAIN}/success?session_id={CHECKOUT_SESSION_ID}`,
    cancel_url: `${process.env.DOMAIN}/cancel`,
    metadata: {
      userId,
    },
  });

  return session;
}
```

## Database Schema

```sql
-- Users table
create table users (
  id uuid references auth.users primary key,
  email text,
  credits integer default 0
);

-- Chats table
create table chats (
  id uuid primary key default uuid_generate_v4(),
  user_id uuid references users(id),
  content text,
  response text,
  created_at timestamp with time zone default timezone('utc'::text, now())
);

-- Credits table
create table credits (
  id uuid primary key default uuid_generate_v4(),
  user_id uuid references users(id),
  amount integer default 0,
  updated_at timestamp with time zone default timezone('utc'::text, now())
);
```

## User Interface Components

### Profile Section
```typescript
// src/components/UserProfile.tsx
export default function UserProfile() {
  const { user } = useAuth();
  const [credits, setCredits] = useState(0);
  const [chats, setChats] = useState([]);

  useEffect(() => {
    if (user) {
      fetchUserData();
    }
  }, [user]);

  return (
    <div className="p-6">
      <h2>Profile</h2>
      <div>Credits: {credits}</div>
      <div>Chat History</div>
      {chats.map(chat => (
        <ChatItem key={chat.id} chat={chat} />
      ))}
    </div>
  );
}
```

### Credits Purchase UI
```typescript
// src/components/PurchaseCredits.tsx
export default function PurchaseCredits() {
  const plans = [
    { credits: 100, price: 10, id: 'price_100' },
    { credits: 500, price: 40, id: 'price_500' },
    { credits: 1000, price: 70, id: 'price_1000' },
  ];

  const handlePurchase = async (priceId) => {
    const session = await createCheckoutSession(user.id, priceId);
    window.location.href = session.url;
  };

  return (
    <div className="grid grid-cols-3 gap-6">
      {plans.map(plan => (
        <PricingCard
          key={plan.id}
          plan={plan}
          onPurchase={() => handlePurchase(plan.id)}
        />
      ))}
    </div>
  );
}
```

## Best Practices & Tips

1. **State Management**
   - Use contexts for global state
   - Keep chat state persistent
   - Handle loading states properly

2. **Error Handling**
   - Implement proper error boundaries
   - Show user-friendly error messages
   - Log errors for debugging

3. **Performance**
   - Implement pagination for chat history
   - Cache API responses
   - Optimize database queries

4. **Security**
   - Secure API endpoints
   - Validate user inputs
   - Protect sensitive data

## Common Issues & Solutions

1. **Chat Persistence**
```typescript
// Save chat state in localStorage
useEffect(() => {
  const savedChats = localStorage.getItem('chats');
  if (savedChats) {
    setMessages(JSON.parse(savedChats));
  }
}, []);
```

2. **Authentication Modal**
```typescript
// Close modal after successful auth
useEffect(() => {
  if (session) {
    setShowAuthModal(false);
  }
}, [session]);
```

3. **Credit System**
```typescript
// Check credits before API call
const handleChat = async () => {
  const hasCredits = await checkCredits(user.id);
  if (!hasCredits) {
    showPurchaseModal();
    return;
  }
  // Process chat...
};
```

## Technical Stack

Here's our complete technical stack:

- **Frontend**: Next.js 14 with App Router
- **Backend**: Edge Functions (Vercel/Cloudflare)
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Payments**: Stripe
- **AI Provider**: OpenAI
- **Analytics**: PostHog
- **Monitoring**: Sentry
- **Testing**: Jest + Playwright

## Development Environment Setup

```bash
# Initial setup
npm create next-app@latest ai-saas --typescript --tailwind
cd ai-saas

# Install dependencies
npm install @supabase/supabase-js stripe openai @vercel/analytics
npm install @tailwindcss/typography @tailwindcss/forms --save-dev

# Environment variables
cp .env.example .env.local
```

### Advanced OpenAI Integration
```typescript:src/lib/openai.ts
import { Configuration, OpenAIApi } from 'openai';
import { rateLimit } from '../utils/rate-limit';

export class AIService {
  private static instance: AIService;
  private openai: OpenAIApi;
  
  private constructor() {
    this.openai = new OpenAIApi(new Configuration({
      apiKey: process.env.OPENAI_API_KEY,
    }));
  }

  static getInstance(): AIService {
    if (!AIService.instance) {
      AIService.instance = new AIService();
    }
    return AIService.instance;
  }

  async processMessage(content: string, context: string[] = []) {
    // Rate limiting check
    const identifier = context[0]?.userId || 'anonymous';
    const rateLimitResult = await rateLimit(identifier);
    
    if (!rateLimitResult.success) {
      throw new Error('Rate limit exceeded');
    }

    try {
      const completion = await this.openai.createChatCompletion({
        model: "gpt-3.5-turbo",
        messages: [
          { role: "system", content: "You are a helpful AI assistant." },
          ...context.map(msg => ({ role: "user", content: msg })),
          { role: "user", content }
        ],
        temperature: 0.7,
        max_tokens: 500,
        presence_penalty: 0.6,
      });

      return completion.data.choices[0].message.content;
    } catch (error) {
      console.error('OpenAI API Error:', error);
      throw new Error('Failed to process message');
    }
  }
}
```

### Rate Limiting Implementation
```typescript:src/utils/rate-limit.ts
import { Redis } from '@upstash/redis';

const redis = new Redis({
  url: process.env.UPSTASH_REDIS_URL,
  token: process.env.UPSTASH_REDIS_TOKEN,
});

export async function rateLimit(identifier: string, limit = 10, window = 60) {
  const key = `rate_limit:${identifier}`;
  
  try {
    const requests = await redis.incr(key);
    
    if (requests === 1) {
      await redis.expire(key, window);
    }

    return {
      success: requests <= limit,
      remaining: Math.max(0, limit - requests),
    };
  } catch (error) {
    console.error('Rate limiting error:', error);
    return { success: true, remaining: limit }; // Fail open
  }
}
```

### Analytics Integration
```typescript:src/lib/analytics.ts
import posthog from 'posthog-js';

export class Analytics {
  static init() {
    if (typeof window !== 'undefined') {
      posthog.init(process.env.NEXT_PUBLIC_POSTHOG_KEY, {
        api_host: process.env.NEXT_PUBLIC_POSTHOG_HOST,
      });
    }
  }

  static trackEvent(event: string, properties?: Record<string, any>) {
    posthog.capture(event, properties);
  }

  static identifyUser(userId: string, traits?: Record<string, any>) {
    posthog.identify(userId, traits);
  }
}
```

## Testing Strategy

```typescript:src/tests/chat.test.ts
import { render, fireEvent, waitFor } from '@testing-library/react';
import Chat from '../components/Chat';

describe('Chat Component', () => {
  it('should handle message sending', async () => {
    const { getByRole, getByText } = render(<Chat />);
    
    const input = getByRole('textbox');
    const sendButton = getByRole('button', { name: /send/i });

    fireEvent.change(input, { target: { value: 'Hello AI' } });
    fireEvent.click(sendButton);

    await waitFor(() => {
      expect(getByText(/Hello AI/)).toBeInTheDocument();
    });
  });
});
```

## Deployment Guide

```yaml:vercel.json
{
  "env": {
    "OPENAI_API_KEY": "@openai_api_key",
    "STRIPE_SECRET_KEY": "@stripe_secret_key",
    "SUPABASE_URL": "@supabase_url",
    "SUPABASE_ANON_KEY": "@supabase_anon_key"
  },
  "build": {
    "env": {
      "NEXT_PUBLIC_SUPABASE_URL": "@supabase_url",
      "NEXT_PUBLIC_SUPABASE_ANON_KEY": "@supabase_anon_key"
    }
  }
}
```

Want to learn more about building AI applications? Follow me for more tutorials and insights! 
