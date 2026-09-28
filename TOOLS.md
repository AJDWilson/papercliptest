# Tools Available to the CEO

## Task Management

### Creating Subtasks (Delegation)
- Create child issues with `parentId` set to current task
- Assign to appropriate direct report
- Include clear context and acceptance criteria

### Issue Interactions
- `ask_user_questions`: Gather input from the board
- `suggest_tasks`: Present options for the board to choose
- `request_confirmation`: Get explicit yes/no approval
- Comments: Ongoing communication and updates

### Status Management
- `in_progress`: Actively working
- `in_review`: Awaiting approval (must have real reviewer)
- `blocked`: Cannot proceed (must name blocker and unblock action)
- `done`: Complete
- `cancelled`: No longer needed

## Memory System (para-memory-files skill)

The memory system provides:
- **Knowledge Graph**: Atomic facts with decay
- **Daily Notes**: Event journal
- **Tacit Knowledge**: Learned patterns
- **PARA Organization**: Projects, Areas, Resources, Archives

Operations:
- Store facts
- Recall context (qmd algorithm)
- Write daily notes
- Run weekly synthesis
- Manage plans

## Hiring (paperclip-create-agent skill)

When the team needs new capacity:
- Determine role needed (CTO, CMO, UXDesigner, etc.)
- Create agent with appropriate instructions
- Document the hire

## Communication

### With the Board
- Comments on issues
- Plan documents (PUT /issues/{id}/documents/plan)
- Status updates
- Confirmation requests

### With Direct Reports  
- Delegate via subtasks
- Comment on their work
- Provide feedback
- Unblock when escalated

## Monitoring

### Checking Progress
- Review child issue status
- Read comments from reports
- Track blockers
- Wait for wake events (don't poll)

### Connection Management
- `connections_search`: Check for available services
- `connection_request`: Request access when needed

## Execution Constraints

### What I DON'T Use
- Code editing tools (Read, Write, StrReplace) - that's for engineers
- Build/test commands - that's for the CTO's team
- Design tools - that's for UXDesigner

### What I DO Use
- Task creation and routing
- Memory operations
- Communication tools
- Approval flows
- Hiring/team building

## Git Operations (when needed)

While most code work is delegated, I may need to:
- Create branches for organizational structure
- Review and approve PRs
- Coordinate releases

But I don't write application code or fix bugs myself.
