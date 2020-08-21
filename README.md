# Steps to reproduce
1. Run `npm i`
2. Run `npm run build`. This will result in the es-abstract type exceptions
3. Changing `compilerOptions.target` to `ES2020` in `tsconfig.json` solves the build exceptions
4. Run `npm run build`.
5. Run `npm run start` shows the exceptions `ES2020` has with optional chaining.

# Desired
No dependency to `ES2020` would solve the issues. `< ES2018` doesnt have the optional chaining issues. But FormatJS forces `ES2020` because of the `es-abstract` dependency.  

