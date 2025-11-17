# New Features - Complete Beginner's Guide

Welcome to Gemini CLI! This guide will help you install, set up, and explore all 10 new features designed to make your experience easier and more productive.

**No technical expertise required** - just follow along step by step!

---

## Table of Contents

1. [Installation](#installation)
2. [First Time Setup](#first-time-setup)
3. [Phase 1: Getting Started](#phase-1-getting-started)
   - [Quick Start Wizard](#1-quick-start-wizard)
   - [Onboarding Dashboard](#2-onboarding-dashboard)
4. [Phase 2: Learning & Discovery](#phase-2-learning--discovery)
   - [Smart Suggestions](#3-smart-suggestions)
   - [Example Library](#4-example-library)
   - [Explain Mode](#5-explain-mode)
5. [Phase 3: Becoming a Power User](#phase-3-becoming-a-power-user)
   - [Tutorial Mode](#6-tutorial-mode)
   - [Workflows](#7-workflows)
   - [Learning Path](#8-learning-path)
6. [Phase 4: Practice & History](#phase-4-practice--history)
   - [Playground](#9-playground)
   - [Command History](#10-command-history)
7. [Troubleshooting](#troubleshooting)

---

## Installation

### Step 1: Install Node.js

Gemini CLI requires Node.js version 18 or higher.

**On Windows:**
1. Go to https://nodejs.org/
2. Download the "LTS" (Long Term Support) version
3. Run the installer
4. Follow the installation wizard (click "Next" through all steps)
5. Restart your computer

**On Mac:**
1. Go to https://nodejs.org/
2. Download the "LTS" version
3. Open the downloaded .pkg file
4. Follow the installation wizard
5. Open Terminal (press Cmd+Space, type "Terminal", press Enter)

**On Linux:**
Open Terminal and run:
```bash
# For Ubuntu/Debian
sudo apt update
sudo apt install nodejs npm

# For Fedora
sudo dnf install nodejs npm

# For Arch Linux
sudo pacman -S nodejs npm
```

**Verify Installation:**
Open your command line/terminal and type:
```bash
node --version
```

You should see something like `v18.0.0` or higher.

### Step 2: Install Gemini CLI

In your command line/terminal, type:
```bash
npm install -g @google/gemini-cli
```

Wait for the installation to complete (this may take 1-2 minutes).

**Verify Installation:**
```bash
gemini --version
```

You should see the version number.

### Step 3: Get Your API Key

You'll need a Google AI Studio API key to use Gemini CLI.

1. Go to https://aistudio.google.com/app/apikey
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy the API key (it looks like a long string of random characters)
5. **Save it somewhere safe** - you'll need it in the next step!

---

## First Time Setup

### Starting Gemini CLI

Open your command line/terminal and type:
```bash
gemini
```

You should see a welcome message and a prompt that looks like this:
```
>
```

This is where you'll type commands!

---

## Phase 1: Getting Started

These features help you set up and learn the basics.

### 1. Quick Start Wizard

**What it does:** Guides you through your first-time setup in just 5 minutes.

**How to use it:**

1. Type this command:
   ```
   /wizard start
   ```

2. You'll see a welcome message. The wizard will guide you through:
   - **Authentication:** Setting up your API key
   - **Workspace:** Choosing your working folder
   - **Preferences:** Customizing your experience
   - **First Task:** Trying your first command

3. Follow the prompts and answer the questions

**Example Session:**
```
> /wizard start

🚀 Welcome to Gemini CLI!

Let's get you set up in just a few minutes.

Step 1: Authentication
Choose your authentication method:
  1. API Key (recommended for beginners)
  2. OAuth (for Google account access)
  3. Vertex AI (for enterprise users)

Progress: 0%
```

**Other wizard commands:**
```
/wizard status    - See your progress
/wizard skip      - Skip the wizard
/wizard reset     - Start over
```

**What to expect:**
- Takes 3-5 minutes to complete
- You'll paste your API key when prompted
- You'll choose a folder to work in
- The wizard saves your preferences automatically

---

### 2. Onboarding Dashboard

**What it does:** Shows you a checklist of 20 tasks to help you learn Gemini CLI features.

**How to use it:**

Type this command:
```
/onboarding
```

You'll see a dashboard with tasks organized into categories:
- **Essential Tasks (6 tasks):** Must-know basics
- **Core Features (8 tasks):** Important features
- **Advanced Features (6 tasks):** Power user skills

**Example Output:**
```
📊 Onboarding Dashboard

Essential Tasks (3/6 completed)
  ✅ Complete Quick Start Wizard
  ✅ Run your first prompt
  ✅ View command history
  ⬜ Try an example
  ⬜ Use file operations
  ⬜ Explore suggestions

Progress: 50%
Next: Try running an example with /examples
```

**Dashboard commands:**
```
/onboarding          - Show dashboard
/onboarding stats    - View detailed statistics
/onboarding reset    - Reset all progress
```

**What to expect:**
- Tasks are auto-detected (checkmarks appear when you complete them!)
- You'll get suggestions for what to try next
- Celebration messages when you complete categories
- Takes 1-2 hours to complete all tasks

---

## Phase 2: Learning & Discovery

These features help you discover what Gemini CLI can do.

### 3. Smart Suggestions

**What it does:** Suggests helpful commands based on what you're working on.

**How to use it:**

1. Turn on suggestions:
   ```
   /suggest enable
   ```

2. View current suggestions:
   ```
   /suggest
   ```

3. The system detects:
   - Git repository status
   - What type of project you're in (Node.js, Python, etc.)
   - Recent files you've changed
   - Commands you've used before

**Example Output:**
```
> /suggest

💡 Smart Suggestions

Based on your Git status:
  📝 "Review my recent changes"
  🔍 "Find files that need updating"
  ✅ "Help me write a commit message"

Based on your project (Node.js):
  🐛 "Check for dependency vulnerabilities"
  📦 "Update outdated packages"
  🧪 "Run my tests"

Tip: Just copy and paste these suggestions!
```

**Suggestion commands:**
```
/suggest              - Show suggestions
/suggest enable       - Turn on suggestions
/suggest disable      - Turn off suggestions
/suggest settings     - View preferences
```

**What to expect:**
- Suggestions update automatically as you work
- The more you use Gemini CLI, the better suggestions get
- Suggestions are context-aware (different for each project)
- You can copy suggestions and use them immediately

---

### 4. Example Library

**What it does:** Provides 50+ ready-to-run examples for common tasks.

**How to use it:**

1. Browse all examples:
   ```
   /examples
   ```

2. Search for something specific:
   ```
   /examples search git
   /examples search "code review"
   /examples search debugging
   ```

3. View example details:
   ```
   /examples show fix-bugs
   ```

4. Run an example:
   ```
   /examples run fix-bugs
   ```

**Example Session:**
```
> /examples

📚 Example Library (50 examples)

⭐ Featured Examples:
  📝 explain-code - Understand complex code
  🐛 fix-bugs - Find and fix bugs automatically
  📊 analyze-data - Analyze data files

Categories:
  💡 Code Understanding (9)
  🔧 Development (9)
  📁 File Operations (9)
  📊 Data Analysis (8)
  📖 Documentation (8)
  ⚙️  Automation (7)

Try: /examples category development
```

**Example commands:**
```
/examples                    - Browse all examples
/examples search <text>      - Search examples
/examples show <id>          - View details
/examples run <id>           - Execute example
/examples category <name>    - Filter by category
/examples featured           - Show featured examples
/examples difficulty beginner - Filter by difficulty
```

**Categories:**
- **Code Understanding:** Review code, find bugs, understand dependencies
- **Development:** Refactoring, testing, optimization
- **File Operations:** Organizing, searching, batch operations
- **Data Analysis:** CSV analysis, JSON processing, statistics
- **Documentation:** Generate docs, README files, API documentation
- **Automation:** Scripting, workflows, batch processing

**What to expect:**
- Each example shows what it does before running
- Examples are safe to run (they won't modify files without asking)
- You can customize examples for your needs
- Examples include helpful explanations

---

### 5. Explain Mode

**What it does:** Shows you what Gemini CLI is doing behind the scenes with helpful explanations.

**How to use it:**

1. Turn on explain mode:
   ```
   /explain on
   ```

2. Now when you use Gemini CLI, you'll see explanations:
   ```
   > Analyze this code for bugs

   🔍 Explain Mode Active

   I'm using these tools:
   - Read: To read your code files
   - Grep: To search for common bug patterns
   - Analysis: To check for logical errors

   Why: Finding bugs requires examining code structure,
   checking for common mistakes, and understanding logic flow.

   💡 Tip: Run tests after fixing bugs to verify the fixes work!
   ```

3. Turn it off when you don't need it:
   ```
   /explain off
   ```

**Explain commands:**
```
/explain on         - Turn on explain mode
/explain off        - Turn off explain mode
/explain status     - Check if it's on or off
/explain settings   - Configure verbosity (brief/normal/detailed)
```

**What to expect:**
- Explanations appear before actions
- You'll learn what each tool does
- Helpful tips and learning suggestions
- No performance impact (explanations are fast)
- Great for learning, can turn off once comfortable

**When to use it:**
- ✅ When learning new features
- ✅ When something doesn't work as expected
- ✅ When you want to understand what's happening
- ⬜ When you're already comfortable (turn it off for cleaner output)

---

## Phase 3: Becoming a Power User

These features help you master Gemini CLI.

### 6. Tutorial Mode

**What it does:** Interactive lessons that teach you Gemini CLI skills step-by-step.

**How to use it:**

1. See available tutorials:
   ```
   /tutorial list
   ```

2. Start a tutorial:
   ```
   /tutorial start basics
   ```

3. The tutorial will:
   - Explain a concept
   - Give you an exercise
   - Check your answer
   - Provide hints if you need help
   - Track your progress

**Example Session:**
```
> /tutorial start basics

📚 Tutorial: Gemini CLI Basics

Lesson 1 of 5: Your First Prompt

In this lesson, you'll learn how to have a conversation with Gemini.

Exercise:
Ask Gemini to explain what a variable is in programming.

Type your answer below, or /tutorial hint for help.

> What is a variable in programming?

✅ Great job! You've completed Lesson 1.

Gemini responded with a clear explanation. Notice how you can
ask questions in natural language - no special syntax needed!

Next lesson: /tutorial next
```

**Tutorial commands:**
```
/tutorial list         - Show all tutorials
/tutorial start <id>   - Start a tutorial
/tutorial next         - Go to next lesson
/tutorial back         - Go to previous lesson
/tutorial hint         - Get a hint
/tutorial solution     - Show solution (gives partial credit)
/tutorial progress     - See your progress
/tutorial quit         - Exit tutorial
```

**Available tutorials:**
1. **basics** - Gemini CLI fundamentals (5 lessons, 15 min)
2. **prompting** - Effective prompting techniques (7 lessons, 20 min)
3. **file-ops** - File operations (6 lessons, 25 min)
4. **code-review** - Code review skills (8 lessons, 30 min)
5. **debugging** - Debugging techniques (7 lessons, 25 min)
6. **refactoring** - Code refactoring (8 lessons, 30 min)
7. **testing** - Writing tests (7 lessons, 25 min)
8. **documentation** - Documentation generation (6 lessons, 20 min)
9. **workflows** - Workflow automation (8 lessons, 30 min)
10. **advanced** - Advanced features (10 lessons, 40 min)

**What to expect:**
- Hands-on learning (you actually do the tasks)
- Immediate feedback on exercises
- Hints available if you get stuck
- Progress saved automatically
- Can pause and resume anytime

---

### 7. Workflows

**What it does:** Automate multi-step tasks with saved workflows.

**How to use it:**

1. Browse available workflows:
   ```
   /workflow list
   ```

2. View workflow details:
   ```
   /workflow show code-review
   ```

3. Run a workflow:
   ```
   /workflow run code-review
   ```

4. Create your own workflow:
   ```
   /workflow create my-workflow
   ```

**Example Session:**
```
> /workflow list

⚙️  Available Workflows (20)

Development:
  📝 code-review - Complete code review process
  🐛 bug-fix - Find and fix bugs
  🧪 test-suite - Create comprehensive tests
  📦 release-prep - Prepare for release

Documentation:
  📖 api-docs - Generate API documentation
  📝 readme - Create README file
  ✍️  changelog - Generate changelog

Try: /workflow show code-review
```

**Workflow commands:**
```
/workflow list           - Show all workflows
/workflow show <id>      - View workflow details
/workflow run <id>       - Execute workflow
/workflow create <name>  - Create new workflow
/workflow edit <id>      - Edit workflow
/workflow export <id>    - Export to file
/workflow import <file>  - Import from file
```

**Popular workflows:**
- **code-review:** Reviews code for bugs, style, performance
- **bug-fix:** Finds bugs, suggests fixes, runs tests
- **test-suite:** Creates comprehensive test coverage
- **refactor:** Improves code structure and readability
- **optimize:** Finds and fixes performance issues
- **document:** Generates documentation from code
- **release-prep:** Prepares code for release (tests, docs, version bump)

**What to expect:**
- Workflows are multi-step automated processes
- You can pause/resume workflows
- Each step shows progress
- Workflows can ask for your input when needed
- Great for repetitive tasks

---

### 8. Learning Path

**What it does:** Gamified learning system with achievements, levels, and skill progression.

**How to use it:**

1. View your learning dashboard:
   ```
   /learning
   ```

2. See your achievements:
   ```
   /learning achievements
   ```

3. Check your current level:
   ```
   /learning stats
   ```

4. View skill tree:
   ```
   /learning skills
   ```

**Example Output:**
```
> /learning

🎯 Learning Path Dashboard

Level: 3 (Intermediate)
XP: 450 / 500 (90% to Level 4)
Streak: 5 days 🔥

Recent Achievements:
  🏆 First Steps - Completed your first tutorial
  💡 Curious Mind - Ran 10 examples
  🔥 On Fire - 5 day streak
  📚 Bookworm - Completed 3 tutorials

Skills Unlocked:
  ✅ Basic Prompting (Level 2)
  ✅ File Operations (Level 1)
  ⬜ Code Review (0/10 XP)
  ⬜ Debugging (0/15 XP)

Next Goal: Complete "Code Review" tutorial (+50 XP)
```

**Learning commands:**
```
/learning                - View dashboard
/learning achievements   - Show all achievements
/learning stats          - Detailed statistics
/learning skills         - View skill tree
/learning goals          - Set learning goals
/learning streak         - View your streak
```

**How to earn XP:**
- Complete tutorials (+50 XP each)
- Run examples (+5 XP each)
- Complete playground challenges (+10-50 XP based on difficulty)
- Unlock achievements (+25-100 XP)
- Maintain daily streaks (+10 XP per day)

**Achievement categories:**
- **Getting Started:** First prompt, first example, wizard completion
- **Explorer:** Try all categories, run 50 examples
- **Scholar:** Complete all tutorials, unlock all skills
- **Challenger:** Complete playground challenges
- **Consistent:** Maintain streaks, daily usage
- **Master:** Reach high levels, master all skills

**What to expect:**
- Fun, game-like progression system
- Clear goals and milestones
- Rewards for consistency (daily streaks)
- Tracks your learning journey
- Motivates you to try new features

---

## Phase 4: Practice & History

These features help you practice skills and track your work.

### 9. Playground

**What it does:** Practice coding with 50 interactive challenges in a safe sandbox environment.

**How to use it:**

1. See available challenges:
   ```
   /playground list
   ```

2. View challenge details:
   ```
   /playground show basic-prompt
   ```

3. Start a challenge:
   ```
   /playground start basic-prompt
   ```

4. Submit your solution:
   ```
   /playground submit basic-prompt
   ```

**Example Session:**
```
> /playground list

🎮 Playground Challenges (50)

Beginner (10 challenges):
  ✅ basic-prompt - Your first prompt (100 pts)
  ⬜ file-search - Find files by pattern (100 pts)
  ⬜ code-explain - Explain code snippet (100 pts)

Intermediate (15 challenges):
  ⬜ bug-detection - Find the bug (200 pts)
  ⬜ code-review - Review code quality (200 pts)

Try: /playground show basic-prompt
```

**Challenge workflow:**

1. **Start:** `/playground start <id>`
   - Read the challenge description
   - Understand the goal
   - Note the test cases

2. **Work on it:**
   - Use Gemini CLI to solve the challenge
   - Test your approach
   - Refine your solution

3. **Get help if stuck:**
   - `/playground hint <id> 0` - Get first hint (-5 pts)
   - `/playground hint <id> 1` - Get second hint (-5 pts)
   - `/playground solution <id>` - View solution (-50% pts)

4. **Submit:** `/playground submit <id>`
   - Your solution is tested automatically
   - Get immediate feedback
   - Earn points if successful

**Playground commands:**
```
/playground list              - Show all challenges
/playground show <id>         - View challenge details
/playground start <id>        - Start a challenge
/playground submit <id>       - Submit your solution
/playground hint <id> <n>     - Get hint (0, 1, 2...)
/playground solution <id>     - View solution
/playground daily             - Get daily challenge
/playground progress          - View your progress
/playground stats             - View statistics
```

**Challenge categories:**
- **Basics (10):** Simple prompts, file operations, basic commands
- **File Operations (15):** File manipulation, searching, organization
- **Data Processing (10):** CSV, JSON, text processing
- **API Integration (5):** Working with APIs and external data
- **Testing (5):** Writing and running tests
- **Debugging (10):** Finding and fixing bugs
- **Optimization (5):** Improving performance
- **Architecture (5):** Design and structure decisions

**Difficulty levels:**
- **Beginner:** 100 points, ~5-10 minutes
- **Intermediate:** 200 points, ~10-20 minutes
- **Advanced:** 300 points, ~20-30 minutes
- **Expert:** 500 points, ~30-60 minutes

**What to expect:**
- Safe sandbox (won't affect your real files)
- Instant feedback on solutions
- Hints available if you get stuck
- Viewing solution gives partial credit (50%)
- Daily challenges for consistent practice
- Leaderboard to track your progress

---

### 10. Command History

**What it does:** Tracks every command you run with powerful search, annotations, and analytics.

**How to use it:**

1. View recent commands:
   ```
   /history list
   ```

2. Search your history:
   ```
   /history search "code review"
   /history search bug
   ```

3. View command details:
   ```
   /history show <id>
   ```

4. Add notes to commands:
   ```
   /history note <id> "This worked great for finding memory leaks!"
   ```

**Example Output:**
```
> /history list

📜 Command History (Last 10)

[2025-11-17 14:32] ✅ Success (2.3s)
  analyze-code src/app.js
  🔖 Bookmarked | ⭐⭐⭐⭐⭐ (5/5)
  📝 Note: Found 3 bugs, very helpful!

[2025-11-17 14:15] ✅ Success (1.1s)
  /examples run fix-bugs

[2025-11-17 13:45] ❌ Error (0.5s)
  invalid-command

[2025-11-17 13:30] ✅ Success (3.7s)
  Review my pull request
  🏷️ Tags: code-review, github

Total commands: 127
Success rate: 94%
```

**Annotation features:**

1. **Bookmark important commands:**
   ```
   /history bookmark <id>
   /history list bookmarked
   ```

2. **Add tags for organization:**
   ```
   /history tag <id> debugging performance
   /history search tag:debugging
   ```

3. **Rate commands:**
   ```
   /history rate <id> 5
   /history list rated:5
   ```

4. **Add notes:**
   ```
   /history note <id> "Useful for analyzing memory usage"
   ```

**Search options:**
```
/history search "text"              - Search by text
/history search tag:debugging       - Search by tag
/history search status:success      - Filter by status
/history search rated:5             - Filter by rating
/history list bookmarked            - Show bookmarked only
/history list date:2025-11-17       - Filter by date
```

**History commands:**
```
/history list                   - Show recent commands
/history search <query>         - Search history
/history show <id>              - View command details
/history bookmark <id>          - Bookmark a command
/history unbookmark <id>        - Remove bookmark
/history tag <id> <tags>        - Add tags
/history untag <id> <tag>       - Remove tag
/history rate <id> <1-5>        - Rate command
/history note <id> <text>       - Add note
/history stats                  - View statistics
/history patterns               - Analyze usage patterns
/history export <format>        - Export (JSON/CSV/Markdown)
```

**Analytics features:**

1. **View statistics:**
   ```
   /history stats
   ```
   Shows:
   - Total commands run
   - Success/error rates
   - Average execution time
   - Most used commands
   - Peak usage times

2. **Pattern detection:**
   ```
   /history patterns
   ```
   Shows:
   - Common command sequences
   - Frequently used workflows
   - Commands often run together
   - Optimization suggestions

3. **Export your history:**
   ```
   /history export json
   /history export csv
   /history export markdown
   ```

**What to expect:**
- Every command is automatically tracked
- Search is instant even with thousands of commands
- Annotations help you remember what worked
- Analytics show your usage patterns
- Export for backup or analysis
- Privacy: stored locally on your computer

**Why it's useful:**
- Remember that command that worked perfectly
- Find patterns in your workflow
- Track your learning progress
- Share helpful commands with teammates
- Learn from your mistakes (see what didn't work)

---

## Troubleshooting

### Command not found

**Problem:** After typing a command, you see "command not found"

**Solution:**
1. Make sure you're inside Gemini CLI (you should see the `>` prompt)
2. Start the command with `/` (slash) - for example `/wizard start` not `wizard start`
3. Check spelling - commands are case-sensitive

### API Key errors

**Problem:** "Invalid API key" or "Authentication failed"

**Solution:**
1. Get a new API key from https://aistudio.google.com/app/apikey
2. Run `/wizard reset` and go through setup again
3. Make sure you copied the entire API key (they're long!)

### Features not showing up

**Problem:** A command returns "Unknown command"

**Solution:**
1. Make sure you installed the latest version:
   ```bash
   npm install -g @google/gemini-cli@latest
   ```
2. Restart Gemini CLI:
   - Type `/quit`
   - Start again with `gemini`

### Slow responses

**Problem:** Commands take a long time to respond

**Solution:**
1. Check your internet connection
2. Some tasks naturally take longer (analyzing large files)
3. The first response is sometimes slower (AI is "warming up")

### Can't find my files

**Problem:** Gemini CLI says it can't find a file

**Solution:**
1. Check you're in the right directory:
   ```
   /pwd
   ```
2. Use full file paths:
   ```
   /Users/yourname/projects/myfile.js
   ```
3. Or navigate to the right folder first

### Reset everything

**Problem:** Something is broken and you want to start fresh

**Solution:**
Run these commands to reset all features:
```
/wizard reset
/onboarding reset
/learning reset
/playground reset
```

Or completely reinstall:
```bash
npm uninstall -g @google/gemini-cli
npm install -g @google/gemini-cli
gemini
```

### Still need help?

1. Check the documentation: Type `/help` in Gemini CLI
2. Run explain mode: `/explain on` to see what's happening
3. Report an issue: Type `/bug` to create a bug report

---

## Quick Reference Card

**Getting Started:**
```
gemini              Start Gemini CLI
/wizard start       Quick setup wizard
/onboarding         View your progress
/help               Get help
/quit               Exit Gemini CLI
```

**Learning:**
```
/examples           Browse 50+ examples
/tutorial list      See available tutorials
/suggest            Get smart suggestions
/explain on         Turn on explanations
/learning           View learning dashboard
```

**Practice:**
```
/playground list    See coding challenges
/playground daily   Today's challenge
/workflow list      Available workflows
```

**Tracking:**
```
/history list       Recent commands
/history search     Find past commands
/history stats      View your statistics
```

---

## Your Learning Journey

Here's a suggested path for learning all features:

**Week 1: Getting Started (30 minutes)**
1. Complete Quick Start Wizard
2. Explore Onboarding Dashboard
3. Run 3-5 examples from the Example Library

**Week 2: Discovery (1 hour)**
1. Turn on Smart Suggestions
2. Enable Explain Mode
3. Complete "Basics" tutorial
4. Try 10 different examples

**Week 3: Building Skills (2 hours)**
1. Complete 3 more tutorials
2. Try your first workflow
3. Complete 5 beginner playground challenges
4. Start tracking your progress in Learning Path

**Week 4: Mastery (3 hours)**
1. Complete all beginner tutorials
2. Try intermediate playground challenges
3. Create your own workflow
4. Explore command history and analytics

**Beyond:**
- Daily: Check daily playground challenge
- Weekly: Complete 1-2 tutorials
- Monthly: Review your history and patterns
- Keep your streak going in Learning Path!

---

## Tips for Success

1. **Start with the wizard** - Don't skip it! It sets everything up correctly.

2. **Use examples liberally** - They're the fastest way to learn what Gemini CLI can do.

3. **Turn on explain mode when learning** - Turn it off when you're comfortable.

4. **Don't be afraid to experiment** - The playground is a safe space to try things.

5. **Track what works** - Use bookmarks and notes in command history to remember helpful commands.

6. **Take tutorials at your own pace** - They're designed to be paused and resumed.

7. **Build a streak** - Using Gemini CLI daily helps you learn faster.

8. **Ask questions naturally** - You don't need special syntax, just ask like you're talking to a person.

9. **Explore all categories** - File operations, code review, testing, documentation - try everything!

10. **Share your learning** - Export your best commands and workflows to share with others.

---

## Congratulations!

You now have everything you need to master Gemini CLI. Start with `/wizard start` and explore from there.

Remember: **Learning is a journey, not a race.** Take your time, explore features at your own pace, and most importantly - have fun!

Happy coding! 🚀
