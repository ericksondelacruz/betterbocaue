# BetterBocaue (Flood Control Capital of the Philippines)

A civic-tech initiative from **Flood Control Capital of the Philippines** providing transparent access to municipal services, programs, and public funds of LGU Bocaue, Bulacan, Philippines.


## About

BetterBocaue.org is a volunteer-driven, open-source project that empowers Bocaueño with easy access to local government information. The platform aggregates public data from official government portals and presents it in a user-friendly, accessible format.

**Cost to the People of Bocaue = ₱0**


## Features

### Public Services Directory

A one-stop guide to LGU services, so residents know where to go and what to do:

- **Health Services** — free check-ups, vaccines, medicines, hospitals, and health programs
- **Education** — daycare/preschool enrollment, scholarships, and education support
- **Business & Livelihood** — permits, clearances, tax and permit payments, and livelihood opportunities
- **Social Welfare** — assistance for seniors, PWDs, solo parents, and indigent families
- **Agriculture & Fisheries** — seeds, fertilizers, veterinary care, training, and equipment lending
- **Infrastructure & Public Works** — reporting damaged roads or drainage, water supply requests, and public facilities
- **Garbage & Waste Disposal** — collection schedules and proper disposal guidelines
- **Environment** — clean-up and tree-planting activities and conservation programs
- **Disaster Preparedness** — emergency plans, response information, and evacuation procedures
- **Housing & Land Use** — housing applications, zoning and building permits, and relocation sites

### Government Information Hub

Everything about the LGU itself, in one place:

- **Departments** — offices with their mandates, services, and contact details
- **News & Announcements** — the latest updates and policy changes
- **Guides & Regulations** — rules and step-by-step instructions for government processes
- **Reports & Statistics** — official reports, data, and performance metrics
- **Public Consultations** — participate and give feedback on local government decisions
- **Transparency Documents** — Freedom of Information releases for public accountability

### Built for Everyone

- **Multilingual** — available in Englis and Filipino
- **Mobile-friendly & accessible** — works well on any phone and is designed for all residents

## Quick Start

### Prerequisites

| Requirement | Version | Purpose                            |
| ----------- | ------- | ---------------------------------- |
| Node.js     | v16+    | Build tools and package management |
| npm         | v8+     | Dependency management              |
| Git         | Latest  | Version control                    |

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/ericksondelacruz/betterbocaue.git
   cd betterbocaue
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

4. **Start development server**

   ```bash
   npm run dev
   ```

5. **Open in browser**
   - Development `http://localhost:5173`
   - Production preview `http://localhost:4173`

## Documentation

- **[CONTENT-GUIDE.md](CONTENT-GUIDE.md)** - Content writing and contribution guidelines
- **[CONTENT-MANAGEMENT.md](CONTENT-MANAGEMENT.md)** - Guide for non-technical users to edit and manage website content
- **[DEPLOYMENT-GUIDE.md](DEPLOYMENT-GUIDE.md)** - Deployment instructions for Vercel and other platforms
- **[CHANGELOG.md](CHANGELOG.md)** - Version history and release notes

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run lint:fix` - Fix ESLint issues
- `npm run format` - Format code with Prettier
- `npm run convert-yaml` - Convert YAML to JSON
- `npm run dev:yaml` - Convert YAML and start dev server

### Project Structure

```
content/
├── government/         # Government section markdown & YAML
│   └── departments/    # Department pages (executive, legislative, etc.)
└── services/           # Services section markdown & YAML

src/
├── components/         # Reusable UI components
│   ├── home/           # Home page components
│   ├── layout/         # Layout components (Navbar, Footer)
│   └── ui/             # Basic UI components
├── data/               # YAML configuration (services.yaml, government.yaml)
├── i18n/               # Internationalization
├── lib/                # Utility functions (markdownLoader, yamlLoader)
├── pages/              # Page components (Home, Services, Government, Document)
└── types/              # TypeScript type definitions
```

## Contributing

We welcome contributions from everyone! Whether you're a developer, government official, or community member, there are many ways to help improve this project.

### For Non-Technical Contributors

**No coding experience required!** You can contribute valuable content and improvements using GitHub's web interface.

#### Quick Start for Non-Technical Users

1. **Create a GitHub account** (free at github.com)
2. **Navigate to the repository** in your web browser
3. **Use our detailed guide**: [CONTENT-MANAGEMENT.md](CONTENT-MANAGEMENT.md) - Complete step-by-step instructions for editing content without any technical knowledge

#### What You Can Contribute

- **Content Updates**: Fix outdated information, add new services, improve descriptions
- **Service Information**: Add details about government services, requirements, and processes
- **Content Review**: Check for accuracy, clarity, and completeness
- **Suggestions**: Propose new features or improvements

#### How to Contribute (No Git Required)

1. **Find content to edit**:
   - Go to `content/services/` for service pages or `content/government/` for department pages
   - Choose a category (health, education, business, departments, etc.)
   - Click on any `.md` file to edit

2. **Make your changes**:
   - Click the pencil icon (✏️) to edit
   - Update the content using simple text formatting
   - Add new information, fix errors, or improve clarity

3. **Save your changes**:
   - Write a brief description of what you changed
   - Click "Commit changes"
   - Your changes will be reviewed and merged

#### Content Types You Can Edit

- **Service Descriptions**: How to apply for permits, scholarships, health services
- **Requirements**: Documents needed, eligibility criteria, deadlines
- **Contact Information**: Office locations, phone numbers, hours
- **Process Steps**: Step-by-step instructions for government services
- **Translations**: Help make content available in local languages

### For Technical Contributors

#### Content Contributors (Basic Technical)

1. **Fork the repository** on GitHub (click "Fork" at https://github.com/ericksondelacruz/betterbocaue)
2. **Clone your fork**: `git clone https://github.com/YOUR-USERNAME/betterbocaue.git`
3. **Add upstream remote**: `git remote add upstream https://github.com/ericksondelacruz/betterbocaue.git`
4. **Create a content branch**: `git checkout -b content/update-health-services`
5. **Edit content files** in `content/`
6. **Test your changes**: `npm run dev`
7. **Submit a pull request** to the original repository

#### Developers

1. **Fork the repository** on GitHub (click "Fork" at https://github.com/ericksondelacruz/betterbocaue)
2. **Clone your fork**: `git clone https://github.com/YOUR-USERNAME/betterbocaue.git`
3. **Add upstream remote**: `git remote add upstream https://github.com/ericksondelacruz/betterbocaue.git`
4. **Create a feature branch**: `git checkout -b feature/new-component`
5. **Make your changes**
6. **Run tests**: `npm run lint && npm run build`
7. **Submit a pull request** to the original repository

#### Keeping Your Fork Updated

To get the latest changes from the original repository:

```bash
# Fetch the latest changes from upstream
git fetch upstream

# Switch to your main branch
git checkout main

# Merge upstream changes into your main branch
git merge upstream/main

# Push updates to your fork on GitHub
git push origin main
```

**Best Practice**: Always sync your fork before creating a new branch for contributions.

### Contribution Guidelines

#### Content Guidelines

- **Accuracy First**: Ensure all information is current and correct
- **Clear Language**: Write for the general public, avoid jargon
- **Complete Information**: Include all necessary details (requirements, steps, contacts)
- **Local Context**: Consider the specific needs of your community
- **Accessibility**: Use clear headings, simple language, and logical structure

#### Technical Guidelines

- Follow existing code style and patterns
- Test your changes thoroughly
- Update documentation when needed
- Ensure mobile responsiveness
- Maintain accessibility standards

### Priority Areas for Contribution

1. **Content Accuracy**: Update outdated information, fix errors
2. **Localization**: Translate content to Filipino
3. **Service Coverage**: Add missing government services and programs
4. **User Experience**: Improve clarity and ease of use
5. **Accessibility**: Ensure content is accessible to all citizens

### Need Help?

- **For Content Questions**: Check [CONTENT-MANAGEMENT.md](CONTENT-MANAGEMENT.md)
- **For Technical Issues**: Open an issue on GitHub
- **For General Questions**: Contact the project maintainers

### Recognition

All contributors are recognized in our project documentation. Your contributions help make government services more accessible to all citizens!

## License

This project is dual-licensed - see the [LICENSE](LICENSE) file for full details:

- **Source code** is licensed under the MIT License.
- **Content and data** (everything under [`content/`](content/)) is licensed under the Creative Commons Attribution 4.0 International License ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).

## Acknowledgments

- Based on the [betterlocalgov](https://github.com/iyanski/betterlocalgov) starter kit
- Built with [React](https://reactjs.org/)
- Styled with [Tailwind CSS v4](https://tailwindcss.com/)
- UI components by [@bettergov/kapwa](https://github.com/bettergov/kapwa)
- Icons by [Lucide React](https://lucide.dev/)
- Content management with [YAML](https://yaml.org/)
- Internationalization with [i18next](https://www.i18next.com/)

---

**PARA SA BAYAN**
