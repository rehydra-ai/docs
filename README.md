# Rehydra Documentation

This is the documentation site for [Rehydra](https://github.com/rehydra-ai/rehydra-sdk), an on-device PII anonymization module for high-privacy AI workflows.

## Documentation Structure

```
docs/
├── index.mdx                    # Introduction
├── quickstart.mdx               # Quick start guide
├── installation.mdx             # Installation for all platforms
├── concepts/
│   ├── pii-types.mdx            # PII types reference
│   ├── anonymization-pipeline.mdx  # How the pipeline works
│   └── encryption.mdx           # Security & encryption
├── guides/
│   ├── ner-detection.mdx        # NER model configuration
│   ├── semantic-enrichment.mdx  # Gender/scope attributes
│   ├── sessions-storage.mdx     # Persistent storage
│   ├── browser-usage.mdx        # Browser-specific guide
│   └── custom-recognizers.mdx   # Custom patterns
└── api-reference/
    ├── introduction.mdx         # API overview
    ├── create-anonymizer.mdx    # createAnonymizer()
    ├── anonymize.mdx            # Anonymize functions
    ├── rehydrate.mdx            # Rehydration functions
    ├── storage-providers.mdx    # Storage providers
    ├── sessions.mdx             # Session API
    ├── crypto.mdx               # Encryption utilities
    └── model-management.mdx     # Model download/cache
```

## Development

### Prerequisites

- Node.js 19+
- [Mintlify CLI](https://www.npmjs.com/package/mintlify)

### Local Preview

```bash
# Install Mintlify CLI
npm i -g mintlify

# Start dev server
cd docs
mintlify dev
```

Visit `http://localhost:3000` to see the docs.

### Deployment

The docs are automatically deployed via the Mintlify GitHub app when changes are pushed to the main branch.

## License

MIT
