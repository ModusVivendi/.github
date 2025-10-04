# Contributing to Modus Vivendi

First off, thank you for considering contributing to Modus Vivendi! Whether you're a team member, mentor, or external contributor, your help is appreciated.

## 🎯 Ways to Contribute

- **Code**: Improve robot code, autonomous routines, or utility tools
- **Documentation**: Write guides, tutorials, or improve existing docs
- **Design**: Create or improve CAD models, schematics, or visual assets
- **Testing**: Help test robot functionality and report bugs
- **Ideas**: Suggest new features or improvements
- **Workshops**: Help create educational content for community outreach

## 📋 Getting Started

### For Team Members

1. **Join the Team Communication Channels**
   - Email: modusvivendior@gmail.com

2. **Set Up Your Development Environment**
   - Install Android Studio for FTC development
   - Install Git and configure your account
   - Clone the relevant repository

3. **Read the Documentation**
   - Check the README of the repository you want to work on
   - Review the project's specific documentation in the `docs/` folder

### For External Contributors

1. **Fork the Repository**
   - Click the "Fork" button on the repository page

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
   cd REPO-NAME
   ```

3. **Add Upstream Remote**
   ```bash
   git remote add upstream https://github.com/ModusVivendi/REPO-NAME.git
   ```

## 🔄 Development Workflow

### 1. Create a Branch

Always create a new branch for your work:

```bash
# For team members
git checkout -b feature/your-feature-name

# For external contributors (from your fork)
git checkout -b feature/your-feature-name
```

Branch naming conventions:
- `feature/description` - New features
- `bugfix/description` - Bug fixes
- `docs/description` - Documentation updates
- `refactor/description` - Code refactoring
- `test/description` - Adding tests

### 2. Make Your Changes

- Write clear, commented code
- Follow the existing code style
- Test your changes thoroughly
- Keep commits focused and atomic

### 3. Commit Your Changes

Write meaningful commit messages:

```bash
git add .
git commit -m "feat(autonomous): add AprilTag detection algorithm

- Implemented OpenCV-based AprilTag detection
- Added distance calculation from detected tags
- Updated autonomous navigation to use tag data
"
```

Commit message format:
```
<type>(<scope>): <subject>

<body>

<footer>
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code formatting (no logic changes)
- `refactor`: Code restructuring
- `test`: Adding tests
- `chore`: Maintenance tasks

### 4. Push Your Changes

```bash
# For team members
git push origin feature/your-feature-name

# For external contributors
git push origin feature/your-feature-name
```

### 5. Create a Pull Request

1. Go to the repository on GitHub
2. Click "New Pull Request"
3. Select your branch
4. Fill out the PR template with:
   - Description of changes
   - Testing performed
   - Related issues (if any)
5. Request review from team leaders

## 📝 Code Style Guidelines

### Java (FTC Projects)

```java
// Use meaningful variable names
double targetDistance = 10.0; // Good
double d = 10.0; // Bad

// Add comments for complex logic
/**
 * Calculates the motor power needed to reach target position
 * using PID control algorithm.
 *
 * @param currentPosition Current encoder position
 * @param targetPosition Desired encoder position
 * @return Motor power value between -1.0 and 1.0
 */
public double calculateMotorPower(int currentPosition, int targetPosition) {
    // Implementation
}

// Use consistent formatting
if (condition) {
    doSomething();
} else {
    doSomethingElse();
}
```

### C++ (Arduino Projects)

```cpp
// Use meaningful names and comments
const int SENSOR_PIN = A0;  // Temperature sensor input
const int LED_PIN = 13;     // Status LED

void setup() {
    pinMode(SENSOR_PIN, INPUT);
    pinMode(LED_PIN, OUTPUT);
}

// Document functions
/**
 * Reads temperature from sensor and returns value in Celsius
 */
float readTemperature() {
    int rawValue = analogRead(SENSOR_PIN);
    return (rawValue * 5.0 / 1024.0 - 0.5) * 100.0;
}
```

## 🧪 Testing Guidelines

### Before Submitting

1. **Test Your Code**
   - Run all existing tests
   - Add new tests for new features
   - Test on actual robot hardware when possible

2. **Check for Issues**
   - No compilation errors
   - No runtime errors in testing
   - Code follows style guidelines

3. **Update Documentation**
   - Update README if needed
   - Add inline code comments
   - Update relevant docs/ files

## 🐛 Reporting Bugs

### Before Reporting

1. Check if the bug has already been reported in Issues
2. Verify the bug exists in the latest version
3. Collect information about the bug

### Creating a Bug Report

Use the bug report template and include:

- **Clear title**: Brief description of the bug
- **Description**: Detailed explanation of the issue
- **Steps to reproduce**: How to trigger the bug
- **Expected behavior**: What should happen
- **Actual behavior**: What actually happens
- **Environment**: 
  - Repository and branch
  - Android Studio version (for FTC)
  - Robot hardware configuration
  - Operating system
- **Screenshots/Logs**: If applicable
- **Possible solution**: If you have ideas

## 💡 Suggesting Features

### Feature Request Template

When suggesting a feature, include:

1. **Problem Statement**: What problem does this solve?
2. **Proposed Solution**: How would you implement it?
3. **Alternatives**: Other approaches considered
4. **Impact**: How would this benefit the team?
5. **Priority**: How urgent is this feature?

## 📖 Documentation

### Writing Documentation

- Use clear, simple language
- Include code examples where helpful
- Add screenshots or diagrams for complex topics
- Keep documentation up to date with code changes

### Documentation Structure

```
docs/
├── README.md              # Overview of documentation
├── SETUP.md              # Setup instructions
├── ROBOT_DESIGN.md       # Hardware specifications
├── PROGRAMMING_GUIDE.md  # Software architecture
├── TROUBLESHOOTING.md    # Common issues and solutions
└── API_REFERENCE.md      # Code API documentation
```

## 🎓 For New Team Members

### Learning Path

1. **Week 1-2: Foundations**
   - Learn Git basics
   - Set up development environment
   - Read team documentation
   - Shadow experienced members

2. **Week 3-4: Small Contributions**
   - Fix minor bugs
   - Update documentation
   - Add code comments
   - Write tests

3. **Week 5+: Major Features**
   - Implement new features
   - Refactor existing code
   - Help mentor newer members

### Getting Help

- Ask questions in team meetings
- Reach out to mentors
- Use GitHub Issues for technical questions
- Check documentation first

## ✅ Pull Request Review Process

### What Reviewers Look For

- **Functionality**: Does it work as intended?
- **Code Quality**: Is it clean and maintainable?
- **Testing**: Is it adequately tested?
- **Documentation**: Is it properly documented?
- **Style**: Does it follow team conventions?

### Review Timeline

- Small PRs (< 50 lines): 1-2 days
- Medium PRs (50-200 lines): 2-4 days
- Large PRs (200+ lines): 4-7 days

### Addressing Review Comments

- Be open to feedback
- Ask questions if unclear
- Make requested changes promptly
- Update PR when ready for re-review

## 🏆 Recognition

We recognize and celebrate contributions:

- Contributors listed in repository README
- Mentions in team social media
- Recognition at team meetings
- Contribution statistics tracked

## 📞 Questions?

If you have questions about contributing:

- **Email**: modusvivendior@gmail.com
- **GitHub Issues**: For technical questions
- **Team Meetings**: For in-person discussions

## 📜 License

By contributing to Modus Vivendi, you agree that your contributions will be licensed under the same license as the project.

---

Thank you for contributing to Modus Vivendi! Together, we're building the future, circuit after circuit. 🤖

**Last Updated**: October 2025  
**Version**: 1.0
