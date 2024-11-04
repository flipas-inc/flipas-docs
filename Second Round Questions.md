# Technical Assessment Questions

## 1. Website/Landing Page Project
Create a website or landing page for your favorite product, company, bar or band
- Complexity, style and tech stack of your choice
- Deliverable: Functional deployed link (e.g. on Vercel)

## 2. Short Answer Questions
Please provide 1-3 paragraphs per question:

- Why do you want to work for Flipas?
- What draws you to computers and technology?
- What is your favorite aspect of programming?
- If you couldn't work in tech, what career would you pursue?

## 3. Technical Problems
Choose one or more of the following problems to solve:

### A. URL Shortener Architecture
Design a scalable URL shortener system
- Deliverable: Architecture diagram + explanation paragraph

### B. Tag Normalization
Given an array of profile tags like: ["JavaScript", "JavaScript", "React", "TypeScript", "react", "REACT"]
Write a function that:
- Removes case-insensitive duplicates
- Normalizes casing (first letter uppercase, rest lowercase) 
- Returns sorted results
- Deliverable: TypeScript function returning ["JavaScript", "React", "TypeScript"]

### C. Chat Interface Component
Design a React chat component handling messages from:
- WebSocket real-time updates
- REST API initial load
- User input

Requirements:
- Maintain message order
- Prevent duplicates
- Handle optimistic updates
- Manage loading states
- Deliverable: Component structure and key hooks

### D. Profile Search Component
You have a profile search component that filters through thousands of profiles:

type Profile = {
  id: string;
  name: string;
  labels: string[];
  location: string;
  lastActive: Date;
}

Users can:
- Search by name
- Filter by multiple labels
- Filter by location
- Sort by last active date

How would you implement this to ensure good performance?
Discuss your approach and any optimizations you'd make.

### E. Job Matching Algorithm
In Flipas's job matching feature, you need to implement a simple recommendation algorithm that matches profiles based on different props:

type UserProfile = {
  skills: Skill[];           // e.g., ["React", "TypeScript"]
  jobPreferences: string[];  // e.g., ["remote", "full-time"]
  experience: number;        // years
  location: string;
  languages: string[];
}

Deliverable: a function that:
a) Takes a target profile and a list of potential matches
b) Returns the top 5 most relevant matches
c) Considers skill matching weight as most important
d) Implements proper TypeScript types
e) Performs efficiently for large datasets

### F. MentorAI Enhancement
Your MentorAI system needs to be enhanced with new capabilities:

1. Function calling to interact with the user's profile data
2. Context-aware responses based on user's CV/skills
3. Multi-modal responses (text + structured data)

type MentorToolCall {
  name: string;
  description: string;
  parameters: Record<string, unknown>;
}

interface MentorResponse {
  message: string;
  metadata?: {
    suggestedSkills?: string[];
    relevantJobs?: JobMatch[];
    confidenceScore?: number;
  };
}

Design a system that:
a) Registers custom tool calls for the OpenAI assistant
b) Handles structured responses with metadata
c) Provides value to the user

Deliverable: Diagram and explanation paragraph
