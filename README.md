from pathlib import Path
import pypandoc

md = r"""# Md. Motaleb Hossain

## Senior Full Stack Developer
**React.js • Next.js • Node.js • PHP • Laravel • WordPress**

Hi, I'm **Motaleb**, a Senior Full Stack Developer with 9+ years of experience building scalable web applications, enterprise WordPress plugins, modern React frontends, and Laravel backends.

### 🚀 Tech Stack
- React.js
- Next.js
- Node.js (Learning)
- JavaScript (ES6+)
- PHP
- Laravel
- WordPress
- WooCommerce
- HTML5
- CSS3
- Bootstrap
- Tailwind CSS
- MySQL
- REST API
- Docker
- Git

### 🌟 Featured Work
- WordPress.org Plugin Author
- Premium Theme Developer
- Custom WordPress Plugin & Theme Development
- AI Integration
- React Admin Dashboards
- REST API Integration

### 💼 Experience
- Riseup Labs – Full Stack WordPress Developer
- Blubird Interactive – WordPress Engineer & Team Lead
- Workspace InfoTech – WordPress & Laravel Developer
- Ifinger Studio – WordPress Developer
- Subra Systems – Software Engineer

### 📫 Connect
- Portfolio: https://motaleb-orcin.vercel.app/
- LinkedIn: https://www.linkedin.com/in/motalebhossain/
- GitHub: https://github.com/motaleb-git
- WordPress.org: https://profiles.wordpress.org/motaleb/
- Email: career.motaleb@gmail.com
"""

out="/mnt/data/README.md"
pypandoc.convert_text(md,'md',format='md',outputfile=out,extra_args=['--standalone'])
print(out)
