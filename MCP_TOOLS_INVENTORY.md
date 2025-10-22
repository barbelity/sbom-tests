# MCP Tools Inventory

This document provides a comprehensive inventory of all Model Context Protocol (MCP) tools available in this environment, with specific focus on JFrog remote MCP tools as requested.

## Executive Summary

**Total MCP Tools Available: ~55 tools**
- **JFrog Remote MCP Tools: ❌ NONE FOUND**
- GitHub MCP Server: 40+ tools
- Playwright Browser: 15+ tools  
- System Tools: 7 tools
- Security Tools: 2 tools

## Detailed Tool Categories

### 1. GitHub MCP Server Tools (40+ tools)
The primary MCP integration providing comprehensive GitHub functionality:

#### Repository Content & Structure
- `github-mcp-server-get_file_contents` - Access files/directories from repositories
- `github-mcp-server-list_branches` - List repository branches
- `github-mcp-server-list_tags` - List git tags
- `github-mcp-server-get_tag` - Get specific tag details

#### Code & Commits
- `github-mcp-server-list_commits` - List commits from branches
- `github-mcp-server-get_commit` - Get commit details with diffs

#### Issues & Project Management
- `github-mcp-server-list_issues` - List issues with filtering
- `github-mcp-server-get_issue` - Get issue details
- `github-mcp-server-get_issue_comments` - Get issue comments
- `github-mcp-server-list_sub_issues` - List sub-issues
- `github-mcp-server-list_issue_types` - List issue types for organizations

#### Pull Requests
- `github-mcp-server-list_pull_requests` - List pull requests
- `github-mcp-server-search_pull_requests` - Search pull requests
- `github-mcp-server-pull_request_read` - Comprehensive PR operations

#### Search Capabilities
- `github-mcp-server-search_code` - Code search across GitHub
- `github-mcp-server-search_issues` - Issue search
- `github-mcp-server-search_repositories` - Repository discovery
- `github-mcp-server-search_users` - User search

#### Security & Scanning
- `github-mcp-server-list_code_scanning_alerts` - Code scanning alerts
- `github-mcp-server-get_code_scanning_alert` - Specific alert details
- `github-mcp-server-list_secret_scanning_alerts` - Secret scanning
- `github-mcp-server-get_secret_scanning_alert` - Secret alert details

#### GitHub Actions & CI/CD
- `github-mcp-server-list_workflows` - List workflows
- `github-mcp-server-list_workflow_runs` - List workflow runs
- `github-mcp-server-get_workflow_run` - Get run details
- `github-mcp-server-get_workflow_run_usage` - Get usage metrics
- `github-mcp-server-get_workflow_run_logs` - Download logs
- `github-mcp-server-list_workflow_jobs` - List workflow jobs
- `github-mcp-server-get_job_logs` - Get job logs
- `github-mcp-server-summarize_run_log_failures` - AI-powered failure analysis
- `github-mcp-server-summarize_job_log_failures` - Job failure summaries

### 2. Playwright Browser MCP Tools (15+ tools)
Complete web automation and testing capabilities:

#### Browser Management
- `playwright-browser_close` - Close browser
- `playwright-browser_resize` - Resize window
- `playwright-browser_tabs` - Tab management
- `playwright-browser_install` - Install browser

#### Navigation & Capture
- `playwright-browser_navigate` - URL navigation
- `playwright-browser_navigate_back` - Back navigation
- `playwright-browser_take_screenshot` - Screenshots
- `playwright-browser_snapshot` - Accessibility snapshots

#### Interaction
- `playwright-browser_click` - Click operations
- `playwright-browser_hover` - Hover actions
- `playwright-browser_drag` - Drag and drop
- `playwright-browser_type` - Text input
- `playwright-browser_press_key` - Keyboard input
- `playwright-browser_select_option` - Dropdown selection
- `playwright-browser_fill_form` - Form filling

### 3. System & Development Tools (7 tools)
Core system operations:

- `bash` - Execute commands (sync/async/detached modes)
- `write_bash` - Send input to bash sessions
- `read_bash` - Read bash output
- `stop_bash` - Stop bash sessions
- `view` - View files and directories
- `create` - Create files
- `str_replace` - Edit files with replacements

### 4. Security Tools (2 tools)
Security scanning and vulnerability detection:

- `gh-advisory-database` - Check GitHub advisory DB for vulnerabilities
- `codeql_checker` - CodeQL security analysis

## JFrog Remote MCP Tools Analysis

### ❌ NO JFROG TOOLS FOUND

After comprehensive analysis of all available MCP tools, **NO JFrog remote MCP tools were detected** in this environment.

#### What JFrog Tools Would Provide
If JFrog MCP tools were available, they would typically include:
- Artifactory repository management
- Xray security scanning
- JFrog Platform APIs
- Binary artifact operations
- Dependency management
- Security policy enforcement

#### How to Add JFrog MCP Integration
To integrate JFrog tools, you would need to:
1. Install a JFrog MCP server package
2. Configure JFrog credentials and endpoints
3. Add JFrog MCP server to your MCP configuration
4. Restart the MCP environment

## Recommendations

1. **For SBOM Testing**: The current GitHub tools provide excellent capability for SBOM workflow testing and repository management.

2. **For JFrog Integration**: If JFrog functionality is required for this SBOM testing repository, consider setting up JFrog MCP tools or using JFrog CLI tools through the bash execution capabilities.

3. **Security**: The existing CodeQL and GitHub Advisory tools provide good security scanning for the current setup.

## Environment Context

This analysis was performed in the `barbelity/sbom-tests` repository, which is described as "a repository to test SBOM integrations." The available tools are well-suited for GitHub-based SBOM testing workflows but lack direct JFrog integration.

---
*Analysis completed on: 2025-10-22*
*Total tools inventoried: ~55*
*JFrog remote MCP tools found: 0*