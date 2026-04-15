web-notes-extension/
│
├── src/
│ ├── background/
│ │ └── service-worker.ts # Handles extension lifecycle, hotkeys, and storage sync
│ ├── content/
│ │ ├── index.tsx # Content script entry point (mounts panel into Shadow DOM)
│ │ └── App.tsx # Main UI root (Tabs, Note Editor, Checklist)
│ ├── components/
│ │ ├── NoteEditor.tsx # Text area with basic formatting controls
│ │ ├── Checklist.tsx # Interactive checklist manager
│ │ └── UrlTabs.tsx # Domain vs. Sub-URL navigation tabs
│ ├── utils/
│ │ ├── storage.ts # Chrome storage wrapper helpers (Typed CRUD)
│ │ └── urlParser.ts # URL normalizer & path classifier
│ └── styles/
│ └── tailwind.css # Tailwind directives scoped to shadow DOM
│
├── public/
│ ├── manifest.json # Extension manifest (v3 config, permissions)
│ └── icons/ # Extension toolbar icons (16x16, 48x48, 128x128)
│
├── package.json # Dependencies & build scripts
├── tsconfig.json # TypeScript configuration
└── tailwind.config.js # Tailwind CSS configuration
