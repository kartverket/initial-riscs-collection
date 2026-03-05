# Repository for Initial RiScs

This repository contains the initial RiScs provided by the RiSc plugin. 
All initial RiScs are located in the `initial-riscs` directory.

The files are stored as JSON.

---

# Editing Initial RiScs

To modify an initial RiSc, update the corresponding file in the `initial-riscs` directory.

Additional configuration for each RiSc is defined in: `init-risc-def.json`
This file contains an array of configuration objects in the following format:

```json
{
  "id": "",
  "priorityIndex": 0,
  "listName": "",
  "listDescription": "",
  "preferredBackstageComponentType": ""
}
```

**‼️An initial RiSc must be defined in init-risc-def.json to be available in the UI ‼️**

- **id**: Specifies the file name of the RiSc. Each RiSc file must follow the naming convention: `<id>.json`.

- **priorityIndex**: Determines the display order of RiScs in the frontend. Lower values indicate higher priority (shown higher in the list).

- **listName**: The name displayed to users when selecting from the available initial RiScs in the frontend.

- **listDescription**: A short description displayed to users when choosing between initial RiScs in the frontend.

- **preferredBackstageComponentType**: Specifies the Backstage component type for which the initial RiSc is intended or recommended.

The file `init-risc-def-schema.json` can be used to verify the `init-risc-def.json` file.