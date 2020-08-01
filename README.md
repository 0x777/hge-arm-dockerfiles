1. Provision an a1 instance (8 Core 16GB seem to suffice) on AWS.
2. Install docker.
3. Build ghc-8.10.1 image for aarch64:
   ```bash
   docker build -t 'ghc:8.10.1-aarch64' -f ghc.df .
   ```
4. Build graphql-engine image for aarch64:
   ```bash
   docker build -t '0x777/graphql-engine:v1.3.0-aarch64' -f hge.df .
   ```
