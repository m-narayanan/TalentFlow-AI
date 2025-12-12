# TalentFlow AI - Intelligent Candidate Screening Platform

An end-to-end recruitment automation system that streamlines candidate screening, conducts AI-powered interviews, and manages hiring workflows.

## Overview

TalentFlow AI solves manual resume screening bottlenecks by automating candidate evaluation through intelligent resume parsing, role-specific AI interviews, and recruiter workflow management. The system integrates multiple technologies to create a cohesive hiring experience.

## Problem It Solves

Traditional hiring involves:
- Manual review of hundreds of resumes
- Inconsistent interview processes
- Time-consuming candidate tracking
- Scattered communication across email and tools

TalentFlow AI centralizes and automates these workflows.

## Key Features

- Automated resume parsing and skill extraction from unstructured text
- AI-driven interview engine that conducts 6-7 question interviews scoring candidates on skills, experience, and communication
- Recruiter dashboard for job posting, candidate review, interview transcript analysis, and approval workflows
- Email and Slack notifications for new applications, interview completion, and shortlist decisions
- Role-specific interview customization based on job requirements
- Candidate profile storage and historical tracking

## Technology Stack

Backend:
- Python with FastAPI framework
- PostgreSQL database for persistent storage
- Groq LLM API for generative AI interview capabilities
- RESTful API architecture

Frontend:
- Streamlit for interactive candidate and recruiter portals
- Real-time data visualization and dashboard

Automation:
- n8n workflow engine for email and Slack integrations
- Webhook-based event processing

## System Architecture

The application follows a modular three-tier architecture:

1. Backend Layer: FastAPI services handling resume parsing, interview orchestration, and candidate management
2. Database Layer: PostgreSQL storing candidates, jobs, interviews, and user data with normalized schema
3. Presentation Layer: Streamlit interfaces for recruiters and candidates with real-time updates

## How It Works

1. Recruiter posts a job opening with role description and required skills
2. Candidates submit applications and resumes
3. System automatically extracts skills and qualifications from resumes
4. AI interview engine conducts role-specific interviews (automatically scheduled)
5. Interview responses scored against job requirements
6. Recruiter reviews candidate profiles, transcripts, and system-generated scores
7. Recruiter approves or rejects candidates
8. Automated notifications sent to candidates and internal team

## Current Status

Core functionality implemented including resume parsing pipeline, interview orchestration, database schema, and basic recruiter workflows. Actively expanding features and deployment capabilities.

## Use Cases

- Startups and mid-size companies looking to automate initial screening rounds
- High-volume recruitment scenarios where manual screening is time-intensive
- Organizations seeking consistent, standardized interview processes
- Remote-first companies needing scalable hiring workflows
