# CoderDojo Oradea Space Robotics - Organization Documentation

<img src="assets/images/logo.png" alt="CoderDojo Oradea Space Robotics Logo" width="150"/>

This repository contains organization-wide documentation, templates, and configuration for all CoderDojo Oradea Space Robotics GitHub projects. It serves as a central location for standardization and resources across all our repositories.

## How We Use GitHub

Our organization uses GitHub for:

1. **Version Control**: All software, hardware designs, and documentation use Git for version tracking
2. **Project Management**: We use Issues and Projects to track tasks and deadlines
3. **Documentation**: Technical guides, design documents, and competition deliverables
4. **Collaboration**: Team members contribute and review each other's work through pull requests
5. **Knowledge Sharing**: Historical record of design decisions and technical approaches

### Repository Types

We maintain several types of repositories:

- **Competition Repositories**: One repository per annual competition (e.g., CanSat2024)
- **Template Repositories**: Reusable templates for documentation and code
- **Learning Repositories**: Training resources for new team members
- **Configuration Repositories**: Organization-wide configuration like this one

## Guidelines for Team Members

### Getting Started

1. **Account Setup**:
   - Create a GitHub account using your personal email
   - Enable 2FA (two-factor authentication)
   - Share your username with the team lead to get added to the organization

2. **Local Environment**:
   - Install Git on your computer
   - Configure Git with your name and email:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "your.email@example.com"
     ```
   - Clone the relevant repositories:
     ```bash
     git clone https://github.com/CoderDojoOradeaSpaceRobotics/CanSat2025.git
     ```

### Workflow

1. **Branches**:
   - `main` - Stable, production-ready code
   - `develop` - Integration branch for ongoing development
   - `feature/feature-name` - For new features
   - `fix/bug-name` - For bug fixes

2. **Commit Messages**:
   - Use present tense ("Add feature" not "Added feature")
   - First line is a summary (max 50 chars)
   - Include the component/subsystem in square brackets, e.g., `[sensors] Add temperature calibration`
   - Reference issue numbers when applicable: `#123`

3. **Pull Requests**:
   - Create PRs for all substantial changes
   - Request reviews from at least one team member
   - PRs should include testing evidence
   - Link to relevant issues

### File Naming Conventions

- Use lowercase with hyphens for spaces (`temperature-sensor.py`)
- Include date in reports (`2025-03-15-progress-report.pdf`)
- Version firmware with semantic versioning (`v1.2.3`)

### Documentation Standards

- All repositories must have a README.md
- Use Markdown for text documentation
- LaTeX for formal reports and papers
- Document code with docstrings and comments
- Include circuit diagrams for hardware

## Development Environment Setup

### Software Requirements

#### Python Development
1. Install Python 3.11 or newer
2. Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

#### Arduino/ESP32 Development
1. Install Arduino IDE or PlatformIO
2. Required libraries:
   - Adafruit Sensor
   - Adafruit BME280
   - TinyGPS++
   - RadioHead

#### PCB Design
1. KiCad 7.0 or newer or Autodesk Eagle
2. Our component libraries (available in Document-templates)

### Hardware Testing

1. Standard test procedures are documented in `/documentation/testing/`
2. Log all test results in the appropriate data folder
3. Include photos of hardware tests when possible

## Internal Resources

- [Team Drive](https://drive.example.com/team) - Shared documents and resources
- [Wiki](https://github.com/CoderDojoOradeaSpaceRobotics/CanSat2025/wiki) - Extended documentation
- [Issue Tracker](https://github.com/orgs/CoderDojoOradeaSpaceRobotics/projects) - Project management
- [LaTeX Templates](https://github.com/CoderDojoOradeaSpaceRobotics/Document-templates) - Standard document formats

## Communication

- Technical discussions: GitHub Issues
- Quick team coordination: Discord
- Weekly status: Team meetings (minutes in Drive)
- External communications: Email

## License

All our repositories are licensed under the MIT License unless otherwise specified.

---

<p align="center">
  <b>For Team Members Only</b><br>
  This documentation is intended for internal use by CoderDojo Oradea Space Robotics team members.
</p>
