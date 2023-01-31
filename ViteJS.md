# Vite JS - Next Generation Frontend Tooling 🚀

- Vite is a Javascript build tool and it is created by Evan You (Creator of Vue)

- It serves your code locally during the development & it bundles your assets, Javascript, and CSS together for production.

- It improves the development experience by focusing on the speed and performance of the build process

## Why is Vite so unique compared to other bundlers?

- Other bundlers like webpack and rollup is also great and work well. But if you are working on a larger application that has more code and dependencies, it takes more time for generating the build and you might have noticed that it takes some time to reflect the change in the browser

- But on the other hand, Vite builds more quickly than other bundlers no matter how large the application is.

## How Vite works?

Traditional bundle-based build tools like Webpack, Rollup, and Parcel, build the entire application before it can be served on the dev-server. This causes slow dev-server cold-start & slow updates.

But Vite completely takes a different approach.

- Vite pre-bundles the app’s dependencies as that does not change often using esbuild (esbuild is built with Golang making 10x-100x faster than other JavaScript bundlers)

- Vite serves source code over native ESM. This allows the browser to take the job of a bundler. Vite only needs to transform and serve source code on demand, as the browser requests it. The code behind conditional dynamic imports is only processed if actually used on the current screen.

- Vite does not re-bundle the whole app if something is changed. It uses route-based code-splitting to determine what part of the code needs to be loaded. It supports Hot Module Replacement (HMR) - allowing a module to "hot replace" itself without affecting the rest of the page.
