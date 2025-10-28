# Project Reflection: Note-Taking App

## Bugs Fixed

### UI/UX Improvements
- **Fixed size elements**: Note list and note context box now have a fixed size
- **Title character limit**: Added validation for long titles without spaces
- **Long title display**: Improved display of long titles in the note list
- **Content formatting**: Fixed issue where multiple lines were combined - now properly separated
- **Horizontal scroll**: Removed unnecessary horizontal scroll bar
- **Save confirmation**: Added prompt asking users to save when starting a new note
- **Delete button timing**: Delete buttons now show only after user saves the note
- **Save button state**: Save button is disabled until there are new changes to the note

## New Features Implemented

### Core Features
- **Tags system**: Added comma-separated tags for note organization
- **Event scheduling**: Added event date and event time fields
- **AI translation**: Integrated AI translate button
- **AI note generation**: Smart note generation that understands temporal context (like "tomorrow") and automatically updates event dates and times

## Technical Challenges & Solutions

### Cloud Database Integration
**Challenge**: Refactor the app to store data in an external database  
**How I solve the Challenge**:
- I use the agent mode in cursor to help me modify the code to use the Supabase cloud database, which guides me step by step to use the cloud database. I met several problems such as how to use the SUPABASE_DB_URL, in order to get the SUPABASE_DB_URL i read through the supabase document and tried many attempts to use the url finally i got everything set up.
- Here is the screenshot that i asked the cursor to help me modify the project to use the cloud database: 
- Connection testing logs and attempts

### Vercel Deployment
**Challenge**: Refactor app structure for successful deployment on Vercel cloud platform  
**Solution**:
- Adapted to Vercel's read-only filesystem (serverless architecture)
- Removed directory creation and SQLite dependencies
- Updated `main.py` to work with Supabase without local file operations
- Created proper `vercel.json` configuration file

### AI Integration
**Challenge**: Implement LLM model for new AI features  
**Solution**:
- Followed lab instructions to deploy GitHub AI using GitHub token
- Used Cursor to implement translate and note generation features
- Integrated AI model with temporal understanding (dates like "tomorrow")

## Technical Implementation

### AI Features
- **Translate button**: AI-powered translation functionality
- **Smart note generation**: AI understands date context and auto-populates event timing
- **Temporal awareness**: AI recognizes and processes date references like "tomorrow"

## Lessons Learned

### Development Process
1. **AI-Assisted Development**: Learned to use AI models for step-by-step full-stack project generation
2. **Problem Solving with AI**: Developed skills in describing bugs and issues effectively for AI troubleshooting
3. **Cloud Deployment**: Gained experience deploying projects with cloud databases and model APIs
4. **Project Publishing**: Understood the complete process from development to publication

### Technical Skills
- Cloud database integration and management
- Serverless architecture constraints and solutions
- AI model integration and API usage
- Full-stack deployment workflows

## Conclusion

This project provided comprehensive experience in modern web development practices, combining cloud infrastructure, AI integration, and responsive deployment strategies. The journey from local development to cloud deployment with AI features demonstrates the current state of full-stack development workflows.
