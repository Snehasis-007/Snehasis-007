# Set up variables
REPO_NAME="Snehasis-Batabyal"
USERNAME="your-github-username"  # Replace with your GitHub username
GITHUB_URL="https://github.com/$USERNAME/$REPO_NAME.git"

# Create the repository on GitHub (Requires GitHub CLI)
gh repo create "$REPO_NAME" --public --confirm

# Clone the new repository
git clone "$GITHUB_URL"
cd "$REPO_NAME"

# Create README.md with formatted content
cat <<EOL > README.md
# Snehasis Batabyal 🚀
### Full-Stack Developer | Open-Source Contributor  

Passionate about technology, coding, and building scalable solutions.  
Pushing boundaries and creating impact with *clean code & innovation*.  

---

## 📌 Tech Stack  
- *Frontend:* HTML, CSS, JavaScript, React  
- *Backend:* Node.js, Express  
- *Database:* MongoDB, MySQL  
- *Tools:* Git, Docker, Postman  

---

### 📫 Connect with Me  
- GitHub: [github.com/SnehasisBatabyal](https://github.com/SnehasisBatabyal)  
- LinkedIn: [linkedin.com/in/snehasisbatabyal](https://linkedin.com/in/snehasisbatabyal)  
- Twitter: [twitter.com/snehasisbatabyal](https://twitter.com/snehasisbatabyal)  
EOL

# Push everything to GitHub
git add .
git commit -m "Initial commit - Snehasis Batabyal"
git push -u origin main
