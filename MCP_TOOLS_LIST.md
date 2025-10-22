# Remote MCP Tools List

This document lists all the remote MCP (Model Context Protocol) tools currently connected and available for use.

## Overview

We have access to **3 main MCP tool servers** with 60+ individual tools:

1. **GitHub MCP Server** (40+ tools) - Comprehensive GitHub API integration
2. **Playwright Browser MCP Server** (15+ tools) - Web automation and testing  
3. **Security Tools** (2 tools) - Vulnerability scanning and analysis

## GitHub MCP Server Tools

### Repository Content & Navigation
- `github-mcp-server-get_file_contents` - Get contents of files or directories from GitHub repositories
- `github-mcp-server-list_branches` - List branches in a GitHub repository
- `github-mcp-server-list_tags` - List git tags in a GitHub repository
- `github-mcp-server-get_tag` - Get details about a specific git tag
- `github-mcp-server-list_commits` - Get list of commits of a branch (30+ results per page)
- `github-mcp-server-get_commit` - Get details for a specific commit with optional diff/stats

### Issues & Pull Requests
- `github-mcp-server-list_issues` - List issues with filtering and pagination (GraphQL-based)
- `github-mcp-server-get_issue` - Get details of a specific issue
- `github-mcp-server-get_issue_comments` - Get comments for a specific issue
- `github-mcp-server-list_sub_issues` - List sub-issues for a specific issue
- `github-mcp-server-list_issue_types` - List supported issue types for organization
- `github-mcp-server-list_pull_requests` - List pull requests with filtering
- `github-mcp-server-pull_request_read` - Comprehensive PR operations (get details, diff, status, files, reviews, comments)

### Labels & Project Management
- `github-mcp-server-list_label` - List labels from repository or specific issue
- `github-mcp-server-get_label` - Get a specific label from repository

### Releases & Distribution
- `github-mcp-server-list_releases` - List releases in a GitHub repository
- `github-mcp-server-get_latest_release` - Get the latest release
- `github-mcp-server-get_release_by_tag` - Get specific release by tag name

### GitHub Actions & CI/CD
- `github-mcp-server-list_workflows` - List workflows in a repository
- `github-mcp-server-list_workflow_runs` - List workflow runs for a specific workflow
- `github-mcp-server-get_workflow_run` - Get details of a specific workflow run
- `github-mcp-server-get_workflow_run_usage` - Get usage metrics for workflow runs
- `github-mcp-server-list_workflow_jobs` - List jobs for a specific workflow run
- `github-mcp-server-get_job_logs` - Download logs for workflow jobs or get all failed job logs
- `github-mcp-server-get_workflow_run_logs` - Download complete workflow run logs (expensive operation)
- `github-mcp-server-list_workflow_run_artifacts` - List artifacts for workflow runs
- `github-mcp-server-download_workflow_run_artifact` - Get download URL for artifacts
- `github-mcp-server-summarize_job_log_failures` - AI-powered analysis of failed job logs
- `github-mcp-server-summarize_run_log_failures` - AI-powered analysis of workflow run failures

### Security & Scanning
- `github-mcp-server-list_code_scanning_alerts` - List code scanning alerts with filtering
- `github-mcp-server-get_code_scanning_alert` - Get details of specific code scanning alert
- `github-mcp-server-list_secret_scanning_alerts` - List secret scanning alerts
- `github-mcp-server-get_secret_scanning_alert` - Get details of specific secret scanning alert

### Search Capabilities
- `github-mcp-server-search_repositories` - Find repositories by name, description, topics, etc.
- `github-mcp-server-search_code` - Fast code search across all GitHub repositories
- `github-mcp-server-search_issues` - Search issues using GitHub's search syntax
- `github-mcp-server-search_pull_requests` - Search pull requests using GitHub's search syntax
- `github-mcp-server-search_users` - Find GitHub users by username, name, or profile info

## Playwright Browser MCP Server Tools

### Navigation & Control
- `playwright-browser_navigate` - Navigate to URLs
- `playwright-browser_navigate_back` - Go back to previous page
- `playwright-browser_resize` - Resize browser window
- `playwright-browser_close` - Close the browser page
- `playwright-browser_tabs` - Manage browser tabs (list, create, close, select)

### Page Interaction
- `playwright-browser_click` - Perform clicks on web elements
- `playwright-browser_hover` - Hover over elements
- `playwright-browser_drag` - Drag and drop between elements
- `playwright-browser_type` - Type text into editable elements
- `playwright-browser_press_key` - Press keyboard keys
- `playwright-browser_select_option` - Select options in dropdowns
- `playwright-browser_fill_form` - Fill multiple form fields at once

### Content Capture & Analysis
- `playwright-browser_snapshot` - Capture accessibility snapshot (better than screenshots)
- `playwright-browser_take_screenshot` - Take page or element screenshots
- `playwright-browser_console_messages` - Get all console messages
- `playwright-browser_network_requests` - Get all network requests since page load

### Advanced Features
- `playwright-browser_evaluate` - Execute JavaScript on page or elements
- `playwright-browser_file_upload` - Upload files through file choosers
- `playwright-browser_handle_dialog` - Handle browser dialogs (alerts, confirms, prompts)
- `playwright-browser_wait_for` - Wait for text appearance/disappearance or time
- `playwright-browser_install` - Install browser if not available

## Security & Vulnerability Tools

### Dependency Security
- `gh-advisory-database` - Check GitHub advisory database for vulnerabilities in dependencies  
  Supports ecosystems: actions, composer, erlang, go, maven, npm, nuget, pip, pub, rubygems, rust, swift

### Code Security
- `codeql_checker` - Discover security vulnerabilities in code using CodeQL analysis

## Additional System Tools

While not remote MCP tools, the following local system tools are also available:

### File System Operations
- `view` - View files and directories with line numbers
- `create` - Create new files with specified content
- `str_replace` - Make precise string replacements in files

### Command Execution
- `bash` - Run Bash commands with sync/async/detached modes
- `write_bash` - Send input to running Bash sessions
- `read_bash` - Read output from async Bash commands
- `stop_bash` - Stop running Bash commands

### Progress Reporting
- `report_progress` - Report progress on tasks and commit changes

---

*Generated on: 2025-10-22*