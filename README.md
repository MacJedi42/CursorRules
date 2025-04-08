Cursor Rules by AI Labs: https://www.youtube.com/@AILABS-393

# Memory Bank for Cursor: Setup & Usage Guide

This guide will help you set up and use Cline's Memory Bank feature with Cursor IDE. Memory Bank helps AI agents maintain context across multiple sessions through structured documentation, reducing context loss and minimising hallucinations.

## Table of Contents
- [The Problem]
- [What is Memory Bank?]
- [Memory Bank File Structure]
- [Workflows]
- [Setup Instructions]
- [Using Memory Bank with Your Projects]
- [Troubleshooting]

## The Problem

During long development sessions, AI agents (like those in Cursor or Windsurf) tend to:
- Forget past conversations
- Lose context between sessions
- Require repeated explanations
- Fill up their context window with redundant information
- Potentially generate hallucinations due to context loss

Memory Bank addresses these issues by maintaining structured documentation that persists across sessions.

## What is Memory Bank?

Memory Bank is a feature originally developed by Klein that:
- Stores structured documentation files to help AI retain context
- Works across multiple sessions, preventing context loss
- Reduces the need to repeatedly explain project details
- Prevents context window overflow
- Minimises AI hallucinations
- Includes built-in task management
- Can be integrated with Cursor IDE

## Memory Bank File Structure

Memory Bank consists of several core files that build upon each other:

1. **Project Brief** (`projectbrief.md`)
   - Outlines the main goals and requirements of the project
   - Serves as the foundation document

2. **Product Context** (`productContext.md`)
   - Explains the problem being solved
   - Describes how the project functions
   - Outlines user experience goals

3. **System Patterns** (`systemPatterns.md`)
   - Documents the architecture and design approach
   - Captures key technical decisions
   - Maps component relationships

4. **Tech Context** (`techContext.md`)
   - Lists the tech stack and dependencies
   - Prevents technical mistakes (e.g., avoids using React Router in a Next.js project)
   - Documents development setup

5. **Active Context** (`activeContext.md`)
   - Tracks what you're currently working on
   - Documents recent changes and next steps

6. **Progress** (`progress.md`)
   - Documents the entire development cycle
   - Tracks completed tasks and upcoming work
   - Documents known issues

## Workflows

Memory Bank operates with two primary workflows:

### Plan Mode
In this mode, the agent:
1. Reads the Memory Bank files
2. Decides what to do next based on stored context
3. Develops a strategy
4. Presents an approach

### Act Mode
In this mode, the agent:
1. Checks the Memory Bank
2. Updates its tasks
3. Takes action on the current task
4. Updates documentation based on what happened

## Setup Instructions

### Getting the Memory Bank Template

1. Go to the raw Memory Bank template markdown file
2. Click on the "Raw" button to view the file in its raw format
3. Copy the entire file content

### Adding to Cursor

1. Open Cursor IDE
2. Navigate to the rules section:
   - For global rules: Go to the global rules settings
   - For project-specific rules: Set up project configuration (tutorials available)

3. Paste the copied Memory Bank template into the rules section

### Initialising Memory Bank for a Project

1. Open your project in Cursor
2. Make sure Cursor Agent mode is enabled
3. Ask Cursor to initialise the Memory Bank:
