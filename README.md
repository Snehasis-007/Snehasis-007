# Set up variables
REPO_NAME="Snehasis-Batabyal"
USERNAME="Snehasis-007"  # Your GitHub username
GITHUB_URL="https://github.com/$USERNAME/$REPO_NAME.git"

# Create the repository on GitHub (Requires GitHub CLI)
gh repo create "$REPO_NAME" --public --confirm

# Clone the new repository
git clone "$GITHUB_URL"
cd "$REPO_NAME"

# Create README.md with a more engaging and structured format
cat <<EOL > README.md
# Snehasis Batabyal 🚀
### Code. Design. Explore. Repeat.  

A normal guy who just loves to code. But give me a chance, and I'll step out to explore the world too.   
Web dev, UI/UX, and C programming are my current playgrounds.  

---

## 🛠️ Tech Stack  
- **Frontend:** HTML, CSS, JavaScript, React  
- **Backend:** Node.js, Express  
- **Database:** MongoDB, MySQL  
- **UI/UX:** Figma, Adobe XD  
- **Programming:** C, JavaScript  
- **Tools:** Git, Docker, Postman  

---

## 🔗 Connect with Me  
- **GitHub:** [github.com/Snehasis-007](https://github.com/Snehasis-007)  
- **LinkedIn:** [linkedin.com/in/snehasisbatabyal](https://linkedin.com/in/snehasisbatabyal)  
- **Twitter:** [twitter.com/snehasisbatabyal](https://twitter.com/snehasisbatabyal)  

EOL

# Push everything to GitHub
git add .
git commit -m "Initial commit - Snehasis Batabyal 🚀"
git push -u origin main
