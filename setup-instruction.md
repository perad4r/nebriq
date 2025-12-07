# Local Setup Instructions

Follow these steps to run Nebriq locally.

1. **Install prerequisites**
   - Node.js 18 or later
   - [Bun](https://bun.sh/)
   - Access to a PostgreSQL database (e.g., Supabase) and API keys for OpenAI and Pinecone.

2. **Clone the repository**
   ```bash
   git clone https://github.com/paulbgtr/nebriq.git
   cd nebriq
   ```

3. **Copy environment variables template**
   ```bash
   cp .env.example .env
   ```
   Fill in the values for OpenAI, Hugging Face, Supabase/PostgreSQL, Pinecone, Polar, and Resend as needed for your environment.

4. **Install dependencies**
   ```bash
   bun install
   ```

5. **Prepare the database**
   - If using Supabase: apply the migrations in the `supabase/` directory to your project.
   - If using local PostgreSQL: create a database and apply the schema from the migrations that fit your setup.

6. **Start the development server**
   ```bash
   bun dev
   ```

7. **Open the app**
   Visit `http://localhost:3000` in your browser to load the Nebriq frontend.
