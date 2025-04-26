# Biometric-Based-Secure-Key-Establishment-for-Secure-Communication

For ibe_dh-main do:
React + TypeScript + Vite.
This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

@vitejs/plugin-react uses Babel for Fast Refresh
@vitejs/plugin-react-swc uses SWC for Fast Refresh
Expanding the ESLint configuration
If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

export default tseslint.config({
  extends: [
    // Remove ...tseslint.configs.recommended and replace with this
    ...tseslint.configs.recommendedTypeChecked,
    // Alternatively, use this for stricter rules
    ...tseslint.configs.strictTypeChecked,
    // Optionally, add this for stylistic rules
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
You can also install eslint-plugin-react-x and eslint-plugin-react-dom for React-specific lint rules:

// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
Commands to run docker
Build image
git clone https://github.com/sahilmk/ibe_dh.git

cd ibe_dh

npm install

npm run dev

Run container
docker run -p 8080:80 my-vite-app

Commands to run docker
Build image
docker build -t my-vite-app .

Run container
docker run -p 8080:80 my-vite-app

Diffie hellman logic
#end



For ns_project_backend-master do:
pip install -r requirements.txt

source venv/bin/activate (Optional)

uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
