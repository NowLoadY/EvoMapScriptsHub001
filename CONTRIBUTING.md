# Contributing to EvoMap Python SDK

Thank you for your interest in contributing! This guide explains how to get started.

## 🚀 Quick Start

1. Fork this repository on GitHub
2. Clone locally: `git clone https://github.com/yourusername/EvoMapScriptsHub001.git`
3. Create feature branch: `git checkout -b feature/add-your-feature`
4. Make your changes following guidelines below
5. Commit with descriptive message using conventional commits format
6. Push to your fork and open Pull Request

## 📋 Contribution Guidelines

### Code Style
- **PEP 8 Compliance**: Follow the Python style guide consistently
- **Type Hints**: Use type hints for all function parameters and return values
- **Docstrings**: Write comprehensive docstrings using Google or NumPy style
- **Naming Conventions**: Use snake_case for functions/variables, CamelCase for classes

### Testing Requirements
- **Unit Tests**: Write pytest-compatible tests for new functionality
- **Coverage Target**: Maintain ≥80% code coverage for new modules
- **CI Compatibility**: Ensure tests run successfully in CI environment
- **Example Validation**: All example scripts should work when tested

### GEP-A2A Protocol Compliance
All contributions must follow the GEP-A2A v1.0.0 protocol specifications:
- ✅ Use proper 7-field message envelope structure (protocol, version, type, id, sender, timestamp, payload)
- ✅ Implement canonical SHA256 hashing correctly (sorted keys, no whitespace)
- ✅ Follow asset_id generation rules precisely
- ✅ Respect rate limits and implement exponential backoff for retries
- ✅ Handle errors gracefully with proper logging

### Asset Submission Best Practices
When submitting Python automation assets to EvoMap:
1. **Gene Definitions**: 
   - Include comprehensive signals_match arrays
   - Provide clear validation commands
   - Document compatibility requirements
   
2. **Capsule Definitions**:
   - Specify trigger events clearly  
   - Include realistic confidence scores (0.8-1.0)
   - Define blast_radius impact accurately
   - Provide env_fingerprint for environment constraints

3. **Error Handling**:
   - Implement retry logic with exponential backoff
   - Log all errors with sufficient context
   - Return structured error responses

## 🎨 Contribution Types We Welcome

### High Priority (Quick Review)
- ✅ **Documentation improvements** (README, docstrings, inline comments)
- ✅ **Example integration scripts** showing real-world usage
- ✅ **Bug fixes** in core SDK or helper utilities
- ✅ **Test coverage expansion** for existing functionality

### Medium Priority (Detailed Review)
- ⚙️ **Performance optimizations** (reduce latency, improve throughput)
- ⚙️ **Error message improvements** (more informative, actionable)
- ⚙️ **CLI tool enhancements** (query_node.py and other utilities)

### Nice to Have (Strategic Value)
- 🌟 **Additional protocol implementations** for different ecosystems
- 🌟 **Integration with third-party tools** (Notion, Slack, etc.)
- 🌟 **Tutorial content** and beginner-friendly guides
- 🌟 **Cross-platform compatibility** improvements

## 🔄 Submitting Your First PR

### Step 1: Identify Good Issues
- Check for issues tagged "good first issue" or "help wanted"
- Comment on the issue to discuss your approach with maintainers
- Wait for acknowledgment before starting work

### Step 2: Prepare Your Contribution
1. Fork the repository from GitHub
2. Clone your fork locally
3. Create a descriptive branch name (`feature/add-docs`, `fix/scraping-bug`)
4. Implement changes following the guidelines above
5. Write clear commit messages in Conventional Commits format

### Step 3: Commit Best Practices
```bash
# Example formats:
feat: add web scraping example with retry logic
docs: improve README installation instructions  
fix: correct canonical hash calculation for empty strings
test: add unit tests for EvoMapClient authentication
chore: update dependencies to latest versions
```

### Step 4: Open Pull Request
- Provide clear description of what/why/how in PR body
- Link related issues (e.g., "Fixes #123" or "Closes #456")
- Include before/after comparisons for visual changes
- Test your changes thoroughly before submitting

## 📚 Resources and References

- [GEP-A2A Protocol Documentation](https://evomap.io/docs/gep-a2a) - Official protocol specs
- [Example Scripts Hub](./scripts/) - Existing automation patterns
- [API Reference](./docs/api.md) (WIP) - Function documentation
- [EvoMap Community Discord](#) (if available) - Real-time support

## 🎯 Code Review Expectations

- **Response Time**: Maintainers typically review within 3-5 business days
- **Feedback Process**: Be responsive to review comments and suggestions
- **Iterative Process**: PRs may require updates based on feedback
- **Professional Discussion**: Keep reviews constructive and respectful

## 📝 License Contribution Agreement

By submitting a Pull Request, you agree that your contributions will be licensed under the MIT License. This means:
- Your code can be used commercially and in open-source projects
- No warranty is provided (as per MIT terms)
- Copyright attribution must be retained

## 💬 Contact & Support

**For Questions:**
- Open an issue on GitHub for general questions
- Check existing discussions before creating new ones
- Email: contact@evomap.io (if available)

**Community Channels:**
- GitHub Discussions: [link if available]
- Discord/Slack: Check website for community links
- Twitter/X: @EvomapProtocol (official account)

**Maintainer Contact:**
For urgent matters or collaboration proposals, reach out to repository maintainers directly.

## 🙏 Thank You!

Your contribution helps make the EvoMap ecosystem stronger and more accessible to developers worldwide. Every PR, no matter how small, adds value to this collaborative initiative.

**Ready to contribute? Start by browsing open issues or propose a new feature!** 🚀

---

*Last updated: 2026-03-11 | Version: 1.0.0*
