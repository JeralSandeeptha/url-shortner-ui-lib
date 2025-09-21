# 📦 Jobber Shared Library

- A shared React UI library containing common reusable components

# ✨ Features
- ✅ UI Components

# 📥 Installation
- Install the package into your microservice:
```cmd
npm install @jeralsandeeptha/jobber-shared
```

# 🚀 Usage
```ts
import { AuthPayload } from '@jeralsandeeptha/jobber-shared';

const user: AuthPayload = {
  id: '123',
  email: 'user@example.com',
  username: 'john_doe'
};
```

# 📂 Project Structure
```cmd
jobber-shared/
├── src/
│   ├── cloudinary.ts
│   ├── error-handler.ts
│   ├── gateway-middleware.ts
│   ├── helpers.ts
│   ├── interfaces/
│   │   ├── auth.interface.ts
│   │   ├── buyer.interface.ts
│   │   ├── ...
│   └── logger.ts
├── cjs/  # Compiled CommonJS
├── esm/  # Compiled ES Modules
└── package.json
```

# 🔧 Development
- Clone the repo and install dependencies:
```cmd
git clone https://github.com/JeralSandeeptha/jobber-shared.git
cd jobber-shared
npm install
```
- Build the package:
```cmd
npm run build
```
- Run tests:
```cmd
npm test
```

- After that make sure to add `.npmrc` file to the root folder if not please add this file. By default this is a github package so we need to specify this is not a npm registry package. That's why we need to do that 
```js
@jeralsandeeptha:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=${NPM_TOKEN}
```

# 📦 Publishing
- Already setup the github actions pipeline for the deployment for the npm registry
- If you want to publish a new version of this package, then after the changes added make sure to change the version that defined in the `package.json` file

# 🤝 Contributing
- Fork the repo
- Create a feature branch (`git checkout -b feature/new-utility`)
- Commit changes (`git commit -m 'Add new utility'`)
- Push branch & open a PR

# 📜 License
MIT © [Jeral Sandeeptha](https://jeral.onrender.com/)