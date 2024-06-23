# Ant Design Pro Template with Login and Registration Only
## Initialization Steps
### Step 1: Delete Directory

Remove the `imagedada-backend` directory in the `src/services` folder:
```bash
rm -rf src/services/imagedada-backend
```

### Step 2: Modify OneAPI Configuration

Update the OneAPI configuration to generate interface code. The backend must adhere to this specification.
Open the config/config.ts file and modify it as follows:
```ts
openAPI: [
  {
    requestLibPath: "import { request } from '@umijs/max'",
    schemaPath: 'http://localhost:8400/api/v2/api-docs',
    projectName: 'imagedada-backend',
  },
]
```

### Step 3: Execute Command

Execute Command in package.json
```json
{
    "openapi" : "max openapi"
}
```

### step 4: Change the method name in the login registration page
