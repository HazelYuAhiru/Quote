## Setup

### Cloning

Clone this repository to your local machine by running the command below:

```bash
git clone [will do later]
```

If you are unfamiliar with `git`, we recommend that you become familiar
with it as soon as possible!

Once you've cloned this repository, you'll need to install some dependencies for the frontend client and the backend API.

### Frontend Setup

Install the dependencies in the frontend directory with `npm` or `yarn`:

```bash
cd frontend
npm ci
```

### Backend Setup

For the Python dependencies, we recommend creating a virtual enviroment:

```bash
python3 -m venv .venv
```

To activate the environment, run the appropriate command for your operating system:

#### Windows

```bat
.\.venv\Scripts\activate
```

#### macOS/Unix

```bash
source .venv/bin/activate
```

Finally, use `pip` to install the required libraries for the backend:

```bash
pip install -r requirements.txt
```

## Development

To start development, launch the development servers on the frontend and backend.
Both development servers also support hot reload, so the instances are refreshed
whenever relevant files are modified.

### Starting the frontend development server

```bash
cd frontend
npm run dev
```

This will start Vite's development server, and the frontend should now be
accessible at `http://localhost:5173`.

### Starting the backend development server

```bash
cd api
python3 src/main.py
```

This will start a Uvicorn server to run the FastAPI app on port 8000.
