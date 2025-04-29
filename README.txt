jlint
------------
This script acts as a git pre-commit hook to validate JMeter (*.jmx) files
for common syntax errors before allowing them to be committed. It checks for:
- Unclosed simple property references (${property})
- Unclosed __P function calls (${__P(param)})
- JSON structure issues when JMeter variables are used in JSON

Installation
------------
1. Copy this script to your repository's .git/hooks directory as 'pre-commit'
2. Make it executable: chmod +x .git/hooks/pre-commit


Usage
-----
The script runs automatically on git commit. (To run manually: ./pre-commit)
