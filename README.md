CreativeForge AI Studio
A production-grade multimodal AI creative platform built with React 19, Vite 8, TypeScript, FastAPI, and Python 3.13.
20 AI-powered creative tools unified under a sleek dark-themed dashboard featuring real-time workflows, node-based pipelines, and dual mock/production execution modes.
 
Live (Local): http://localhost:3000 (Frontend) | http://localhost:5000 (API)

Table of Contents

Features
Tech Stack
Architecture
Getting Started
Project Structure
Mock vs Production Mode
Key Capabilities
Deployment
Future Roadmap
Contributing
License


Features
CreativeForge delivers 20 specialized AI creative tools:

Creative Memory Engine (RAG) — Personalized generation using vector memory (pgvector)
AI Creative Director — Prompt analysis and intelligent enhancement
Live Canvas — Real-time collaborative canvas with co-creation
AI World Engine — Consistent story worlds, characters & continuity validation
Emotional AI Generation — Mood-aware visual generation
AI Style Genome System — Evolving personal artistic fingerprint
AI Render Preview — Real-time render job monitoring
AI Asset Management — Smart organization, tagging & collections
AI Prompt-to-Product — Turn prompts into refined products
AI Multi-Modal Fusion — Combine text, image & audio
Cinematic AI Director — Professional camera, lighting & grading controls
AI Knowledge Graph — Entity-relation graphs for world-building
Generative UI — AI-generated interface components
AI Marketplace Ecosystem — Buy/sell prompts, assets & styles
AI Timeline & Versioning — Full project history and version control
Voice-Driven Creation — Hands-free voice command interface
Real-Time Collaborative Studio — Multi-user WebRTC collaboration
Personal AI Creative Twin — AI that learns your creative style
AI Research & Inspiration Engine — Track papers and inspirations
Future-Ready Expansions — Built-in roadmap & planning tools

Visual Node Workflow System — Drag-and-drop pipeline builder powered by ReactFlow.

Tech Stack


















































LayerTechnologyVersionFrontendReact + Vite + TypeScript19 / 8StateZustand5.xWorkflowsReactFlow11.xBackendFastAPI + PythonLatest / 3.13ORMSQLModel (SQLAlchemy + Pydantic)-DatabasePostgreSQL + pgvector15+QueueRedis (Celery/RQ)-AuthJWT-
Additional: Framer Motion, Three.js/Pixi.js, Tailwind-free (inline styles).

Architecture
#mermaid-diagram-mermaid-pk0f39b{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#ccc;}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#mermaid-diagram-mermaid-pk0f39b .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#mermaid-diagram-mermaid-pk0f39b .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#mermaid-diagram-mermaid-pk0f39b .error-icon{fill:#a44141;}#mermaid-diagram-mermaid-pk0f39b .error-text{fill:#ddd;stroke:#ddd;}#mermaid-diagram-mermaid-pk0f39b .edge-thickness-normal{stroke-width:1px;}#mermaid-diagram-mermaid-pk0f39b .edge-thickness-thick{stroke-width:3.5px;}#mermaid-diagram-mermaid-pk0f39b .edge-pattern-solid{stroke-dasharray:0;}#mermaid-diagram-mermaid-pk0f39b .edge-thickness-invisible{stroke-width:0;fill:none;}#mermaid-diagram-mermaid-pk0f39b .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-diagram-mermaid-pk0f39b .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-diagram-mermaid-pk0f39b .marker{fill:lightgrey;stroke:lightgrey;}#mermaid-diagram-mermaid-pk0f39b .marker.cross{stroke:lightgrey;}#mermaid-diagram-mermaid-pk0f39b svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-diagram-mermaid-pk0f39b p{margin:0;}#mermaid-diagram-mermaid-pk0f39b .label{font-family:"trebuchet ms",verdana,arial,sans-serif;color:#ccc;}#mermaid-diagram-mermaid-pk0f39b .cluster-label text{fill:#F9FFFE;}#mermaid-diagram-mermaid-pk0f39b .cluster-label span{color:#F9FFFE;}#mermaid-diagram-mermaid-pk0f39b .cluster-label span p{background-color:transparent;}#mermaid-diagram-mermaid-pk0f39b .label text,#mermaid-diagram-mermaid-pk0f39b span{fill:#ccc;color:#ccc;}#mermaid-diagram-mermaid-pk0f39b .node rect,#mermaid-diagram-mermaid-pk0f39b .node circle,#mermaid-diagram-mermaid-pk0f39b .node ellipse,#mermaid-diagram-mermaid-pk0f39b .node polygon,#mermaid-diagram-mermaid-pk0f39b .node path{fill:#1f2020;stroke:#ccc;stroke-width:1px;}#mermaid-diagram-mermaid-pk0f39b .rough-node .label text,#mermaid-diagram-mermaid-pk0f39b .node .label text,#mermaid-diagram-mermaid-pk0f39b .image-shape .label,#mermaid-diagram-mermaid-pk0f39b .icon-shape .label{text-anchor:middle;}#mermaid-diagram-mermaid-pk0f39b .node .katex path{fill:#000;stroke:#000;stroke-width:1px;}#mermaid-diagram-mermaid-pk0f39b .rough-node .label,#mermaid-diagram-mermaid-pk0f39b .node .label,#mermaid-diagram-mermaid-pk0f39b .image-shape .label,#mermaid-diagram-mermaid-pk0f39b .icon-shape .label{text-align:center;}#mermaid-diagram-mermaid-pk0f39b .node.clickable{cursor:pointer;}#mermaid-diagram-mermaid-pk0f39b .root .anchor path{fill:lightgrey!important;stroke-width:0;stroke:lightgrey;}#mermaid-diagram-mermaid-pk0f39b .arrowheadPath{fill:lightgrey;}#mermaid-diagram-mermaid-pk0f39b .edgePath .path{stroke:lightgrey;stroke-width:2.0px;}#mermaid-diagram-mermaid-pk0f39b .flowchart-link{stroke:lightgrey;fill:none;}#mermaid-diagram-mermaid-pk0f39b .edgeLabel{background-color:hsl(0, 0%, 34.4117647059%);text-align:center;}#mermaid-diagram-mermaid-pk0f39b .edgeLabel p{background-color:hsl(0, 0%, 34.4117647059%);}#mermaid-diagram-mermaid-pk0f39b .edgeLabel rect{opacity:0.5;background-color:hsl(0, 0%, 34.4117647059%);fill:hsl(0, 0%, 34.4117647059%);}#mermaid-diagram-mermaid-pk0f39b .labelBkg{background-color:rgba(87.75, 87.75, 87.75, 0.5);}#mermaid-diagram-mermaid-pk0f39b .cluster rect{fill:hsl(180, 1.5873015873%, 28.3529411765%);stroke:rgba(255, 255, 255, 0.25);stroke-width:1px;}#mermaid-diagram-mermaid-pk0f39b .cluster text{fill:#F9FFFE;}#mermaid-diagram-mermaid-pk0f39b .cluster span{color:#F9FFFE;}#mermaid-diagram-mermaid-pk0f39b div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:12px;background:hsl(20, 1.5873015873%, 12.3529411765%);border:1px solid rgba(255, 255, 255, 0.25);border-radius:2px;pointer-events:none;z-index:100;}#mermaid-diagram-mermaid-pk0f39b .flowchartTitleText{text-anchor:middle;font-size:18px;fill:#ccc;}#mermaid-diagram-mermaid-pk0f39b rect.text{fill:none;stroke-width:0;}#mermaid-diagram-mermaid-pk0f39b .icon-shape,#mermaid-diagram-mermaid-pk0f39b .image-shape{background-color:hsl(0, 0%, 34.4117647059%);text-align:center;}#mermaid-diagram-mermaid-pk0f39b .icon-shape p,#mermaid-diagram-mermaid-pk0f39b .image-shape p{background-color:hsl(0, 0%, 34.4117647059%);padding:2px;}#mermaid-diagram-mermaid-pk0f39b .icon-shape rect,#mermaid-diagram-mermaid-pk0f39b .image-shape rect{opacity:0.5;background-color:hsl(0, 0%, 34.4117647059%);fill:hsl(0, 0%, 34.4117647059%);}#mermaid-diagram-mermaid-pk0f39b :root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}React 19 FrontendFastAPI BackendRedis QueueGPU Inference WorkersAI Models: SDXL, Flux, Mistral, etc.PostgreSQL + pgvector
Core Principles:

Monorepo for shared code
Clear separation: Routers → Services → Repositories
Dual-mode execution (Mock for dev, Production for GPU)
Premium glassmorphism dark UI inspired by RunwayML / Leonardo


Getting Started
Prerequisites

Node.js 18+
Python 3.13+
(Optional) PostgreSQL 15+ and Redis for production mode

1. Clone & Install
Bashgit clone <your-repo-url>
cd CreativeForge

# Root dependencies
npm install --legacy-peer-deps

# Frontend
cd apps/web && npm install --legacy-peer-deps
2. Start Backend (Mock Mode - Recommended for dev)
Bashcd apps/api
python3 main_mock.py
API runs at http://localhost:5000
3. Start Frontend
Bashcd ../..   # back to root
npx vite apps/web --port 3000 --host 0.0.0.0
Dashboard available at http://localhost:3000
Pre-configured mock user: Shawon Admin (admin)

Project Structure
textCreativeForge/
├── apps/
│   ├── web/           # React 19 + Vite frontend
│   └── api/           # FastAPI backend
├── infrastructure/    # Docker, K8s, Terraform
├── docs/              # Architecture & API docs
├── packages/          # Shared types & SDK
└── scripts/
Full detailed structure available in the original README.

Mock vs Production Mode


























ModeDatabaseRedisGPUUse CaseMockIn-memoryNoNoDevelopment & TestingProdPostgreSQL + pgvectorYesYesReal inference & production
Run production with:
Bashcd apps/api && python3 main.py

Key Capabilities

Real-time workflows with node-based pipelines
RAG-powered creative memory for consistent style & context
Dual execution modes for frictionless development
Fully responsive dark UI with glassmorphism
Command Palette (⌘K)
Toast notifications, error boundaries, skeletons
Extensive API coverage for all 20 features


Deployment

Local: Docker Compose (see infrastructure/docker/)
Cloud: Kubernetes + Terraform manifests included
Scaling: Horizontal pod autoscaling, GPU node pools, Blue-Green deployments


Future Roadmap
Short-term: Video generation, batch processing, mobile app, Stripe billing
Medium-term: ComfyUI nodes, model fine-tuning, public API
Long-term: On-premise, 3D generation, global edge inference

Contributing
Contributions are welcome! Please see CONTRIBUTING.md and Code of Conduct.

Fork the project
Create a feature branch
Make changes and test in mock mode
Submit a PR


License
MIT License - see LICENSE file for details.

Built with passion for creative AI workflows.
Star the repo if you find it useful! ⭐
