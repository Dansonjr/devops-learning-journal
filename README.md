
**Key learnings:**
- RDS = managed PostgreSQL in the cloud
- Security groups = cloud firewalls (must allow my IP)
- Public access = Yes needed for external connections
- Always delete resources immediately after testing

**Code sample:** `test_rds.py` in my rds-python-connection repo

**Next:** Day 3 – CloudFormation (Infrastructure as Code)

### Day 2 – Complete ✅

**Date:** [Today]

**What I accomplished:**
- [x] Launched RDS PostgreSQL database in AWS (Free Tier)
- [x] Configured public access and security group for my IP
- [x] Connected from Ubuntu using Python + psycopg2
- [x] Successfully queried PostgreSQL version
- [x] Deleted database after testing (no charges)

**Connection details I used:**


### Git Authentication Lesson

**Problem:** Got "Invalid username or token" when pushing with HTTPS.

**Solution:** Switched remote URL from HTTPS to SSH.

**Commands learned:**
```bash
git remote set-url origin git@github.com:username/repo.git
git remote -v  # verify the change
Save (`Ctrl+O` → Enter → `Ctrl+X`), then:

```bash
git add README.md
git commit -m "Add Git authentication lesson"
git push
# devops-learning-journal
Daily log of my DevOps learning journey
### Python Setup on Ubuntu "Questing"

**Challenge:** deadsnakes PPA doesn't support my Ubuntu version yet.

**Solution:** Used `virtualenv` instead of `venv` – works exactly the same!

**Command learned:**
```bash
sudo apt install python3-virtualenv -y
virtualenv venv -p python3.13
source venv/bin/activate
pip install psycopg2-binary
deactivate

