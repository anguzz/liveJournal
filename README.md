
# Live Journal

This project began in **2023** as a **SvelteKit + Skeleton Labs** site and was deployed on **Vercel**.  
As of **2026**, it has been intentionally migrated to **plain HTML, CSS, and JavaScript**.

## Why the Change

### 1. Template + Dependency Mismatch
The project was scaffolded from a **Skeleton v3-era template**, but dependency upgrades pulled in:

- Skeleton v4
- Tailwind v4
- Vite v7

Skeleton v4 removed global CSS, changed imports, and requires a different structure.  
Mixing an old template with new packages led to unavoidable build failures.

### 2. Deployment Friction (Node Versions)
Vercel builds failed with:

```

Unsupported Node.js version: v24.x
Please use Node 16 or 18

```

This required Node pinning and adapter configuration for a site that does not need a server runtime. It was overengineered for a very simple setup at the time because I was interested in the skeleton framework but it purely has static content, no backend apis, or auth. Framework tooling added complexity without real benefit.


## Current Setup

- Plain HTML
- CSS (Water.css dark theme)
- Alpine.js for minimal interactivity
- Static JavaScript data
- No build step
- No Node runtime
- No framework lock-in

## Summary

After ~3 years of dependency churn, the project was simplified to match its actual scope.  
For this site, **static + minimal JS is the correct tool**.
