# MCP Tools Inventory

This document provides a comprehensive list of all Model Context Protocol (MCP) tools currently connected and available in this environment.

## Executive Summary

- **Total MCP Tools**: 67 tools across 4 main categories
- **GitHub Tools**: 42 tools (comprehensive GitHub API coverage)
- **Playwright Browser Tools**: 19 tools (full browser automation)
- **System & Development Tools**: 4 tools (file/command operations)
- **Security Tools**: 2 tools (vulnerability scanning)
- **JFrog Tools**: ⚠️ **0 tools** (none currently connected)

## GitHub MCP Server Tools (42 tools)

### Workflow & CI/CD Tools
- `github-mcp-server-download_workflow_run_artifact` - Download artifacts from workflow runs
- `github-mcp-server-get_workflow_run` - Get workflow run details
- `github-mcp-server-get_workflow_run_logs` - Download complete workflow logs (EXPENSIVE)
- `github-mcp-server-get_workflow_run_usage` - Get workflow run usage metrics
- `github-mcp-server-list_workflow_jobs` - List jobs for workflow runs
- `github-mcp-server-list_workflow_run_artifacts` - List workflow run artifacts
- `github-mcp-server-list_workflow_runs` - List workflow runs
- `github-mcp-server-list_workflows` - List repository workflows
- `github-mcp-server-get_job_logs` - Download workflow job logs (supports failed_only)
- `github-mcp-server-summarize_job_log_failures` - AI-powered job failure analysis
- `github-mcp-server-summarize_run_log_failures` - AI-powered workflow failure analysis

### Repository Management
- `github-mcp-server-get_file_contents` - Get file/directory contents from repositories
- `github-mcp-server-get_commit` - Get commit details with optional diff/stats
- `github-mcp-server-list_commits` - List commits with pagination
- `github-mcp-server-list_branches` - List repository branches
- `github-mcp-server-get_tag` - Get git tag details
- `github-mcp-server-list_tags` - List git tags
- `github-mcp-server-get_latest_release` - Get latest release information
- `github-mcp-server-get_release_by_tag` - Get release by tag name
- `github-mcp-server-list_releases` - List repository releases

### Issues & Project Management
- `github-mcp-server-get_issue` - Get specific issue details
- `github-mcp-server-get_issue_comments` - Get comments for issues
- `github-mcp-server-list_issues` - List repository issues
- `github-mcp-server-list_issue_types` - List supported issue types
- `github-mcp-server-list_sub_issues` - List sub-issues for specific issues
- `github-mcp-server-get_label` - Get repository labels
- `github-mcp-server-list_label` - List repository or issue labels

### Pull Requests
- `github-mcp-server-list_pull_requests` - List pull requests
- `github-mcp-server-pull_request_read` - Comprehensive PR operations:
  - `get` - Get PR details
  - `get_diff` - Get PR diff
  - `get_status` - Get head commit status
  - `get_files` - Get changed files list
  - `get_review_comments` - Get review comments
  - `get_reviews` - Get reviews

### Security & Scanning
- `github-mcp-server-get_code_scanning_alert` - Get specific code scanning alert details
- `github-mcp-server-list_code_scanning_alerts` - List code scanning alerts
- `github-mcp-server-get_secret_scanning_alert` - Get secret scanning alert details
- `github-mcp-server-list_secret_scanning_alerts` - List secret scanning alerts

### Search & Discovery
- `github-mcp-server-search_code` - Search code across all GitHub repositories
- `github-mcp-server-search_issues` - Search issues using GitHub syntax
- `github-mcp-server-search_pull_requests` - Search pull requests
- `github-mcp-server-search_repositories` - Search repositories by various criteria
- `github-mcp-server-search_users` - Search GitHub users

## Playwright Browser MCP Tools (19 tools)

### Browser Management
- `playwright-browser_close` - Close browser page
- `playwright-browser_resize` - Resize browser window
- `playwright-browser_install` - Install browser if needed
- `playwright-browser_tabs` - Manage browser tabs (list, new, close, select)

### Navigation
- `playwright-browser_navigate` - Navigate to URLs
- `playwright-browser_navigate_back` - Go back in browser history

### Interaction
- `playwright-browser_click` - Click elements (supports modifiers, double-click)
- `playwright-browser_type` - Type text into elements
- `playwright-browser_press_key` - Press keyboard keys
- `playwright-browser_hover` - Hover over elements
- `playwright-browser_drag` - Drag and drop operations
- `playwright-browser_select_option` - Select dropdown options
- `playwright-browser_fill_form` - Fill multiple form fields
- `playwright-browser_file_upload` - Upload files via browser

### Monitoring & Testing
- `playwright-browser_console_messages` - Get console messages
- `playwright-browser_network_requests` - Get network requests
- `playwright-browser_take_screenshot` - Take page/element screenshots
- `playwright-browser_snapshot` - Capture accessibility snapshots
- `playwright-browser_wait_for` - Wait for conditions (text appear/disappear, time)

### Advanced Features
- `playwright-browser_handle_dialog` - Handle browser dialogs
- `playwright-browser_evaluate` - Execute JavaScript in browser

## System & Development Tools (4 tools)

### File Operations
- `view` - View files and directories with line numbers
- `create` - Create new files
- `str_replace` - Make string replacements in files

### Command Execution
- `bash` - Execute bash commands with multiple modes:
  - `sync` - Synchronous execution (default)
  - `async` - Asynchronous execution for interactive tools
  - `detached` - Persistent processes
- `write_bash` - Send input to bash sessions (text + keyboard input)
- `read_bash` - Read output from bash commands
- `stop_bash` - Stop running bash commands

## Security Tools (2 tools)

### Vulnerability Scanning
- `gh-advisory-database` - Check GitHub advisory DB for vulnerabilities
  - **Supported ecosystems**: actions, composer, erlang, go, maven, npm, nuget, other, pip, pub, rubygems, rust, swift
  - **Note**: Only use for supported ecosystems, skip for others (e.g., Haskell/Cabal, C++/vcpkg)
  
- `codeql_checker` - Discover security vulnerabilities using CodeQL
  - Must be run before finalizing tasks
  - Provides security analysis of code changes

## JFrog MCP Tools Status

### ❌ No JFrog Tools Currently Connected

**Current Status**: No JFrog MCP tools are currently available in this environment.

**Missing JFrog Capabilities**:
- Artifactory operations (artifact upload/download, repository management)
- Xray security scanning (vulnerabilities, license compliance)
- Distribution management
- Access control and permissions
- Build integration
- Docker registry operations

**To Add JFrog Support**:
If JFrog functionality is needed, a JFrog MCP server would need to be connected to provide access to:
- JFrog Artifactory
- JFrog Xray  
- JFrog Distribution
- JFrog Access
- JFrog Pipelines
- Other JFrog Platform services

## Custom Agents (2 available)

### Specialized Task Agents
- `readme-drawer` - Agent for drawing cool things in README files
- `sec-agent` - Agent that lists connected MCP tools (used to generate this inventory)

---

*This inventory was generated on 2025-10-22T06:48:50.197Z using the sec-agent MCP tool analyzer.*