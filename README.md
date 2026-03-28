# VanAdhikar – AI-Powered WebGIS and Decision Support System

**VanAdhikar** is a comprehensive, AI-driven platform designed to revolutionize **Forest Rights Act (FRA)** implementation in India. It digitizes legacy claims data, provides real-time geospatial monitoring, maps community assets, and delivers personalized scheme recommendations to tribal communities, creating a **transparent and efficient rights recognition ecosystem**.

---
## My Repository Contributions

The following graph represents my contribution activity to this collaborative repository.

<img width="516" height="248" alt="image" src="https://github.com/user-attachments/assets/3762988e-99be-4af6-a2d2-1650b87b355f" />

---

## **Key Features**:

### **1. AI-Powered Legacy Data Digitization:**
- Automated **OCR + NER pipeline** extracts and standardizes handwritten FRA claims, verification records, and patta documents into structured digital formats.
- **Human-in-the-loop verification** ensures critical data accuracy by combining AI efficiency with manual validation checkpoints.
- **Centralized digital archive** creates a searchable repository of all FRA claims, decisions, and title records accessible to authorized stakeholders.

### **2. Real-Time FRA Atlas & WebGIS Platform:**
- **Interactive geofenced maps** automatically extract coordinates from digitized pattas and generate shapefiles, visualizing granted FRA regions on an exportable atlas.
- **Satellite imagery integration** overlays high-resolution images on geofenced areas for visual validation and continuous monitoring.
- **State-district-village hierarchy** enables intuitive navigation from state level down to individual tribal groups and claim parcels.
- **Real-time status tracking** displays claim status (pending, approved, rejected) with complete audit trails on live dashboards.

### **3. Deep Learning-Based Asset Mapping:**
- **Custom CNN pipeline** identifies and maps forest resources including ponds, farms, water bodies, and vegetation cover within FRA villages using satellite imagery.
- **Automated inventory generation** creates detailed asset inventories for each community forest resource (CFR) and individual forest rights (IFR) area.
- **Change detection** monitors asset changes over time using temporal satellite imagery analysis to track encroachment or degradation.

### **4. AI-Driven Decision Support System (DSS):**
- **FRA Atlas** leverages **AI and multi-parameter analysis** to match eligible tribal individuals and communities with relevant government schemes (MGNREGA, PM-KISAN, PMAY, etc.).
- **Personalized scheme mapping** uses AI to analyze water index (DWLR), geospatial assets, agro-economic data, IoT sensor data, and socio-demographic profiles.
- **Eligibility scoring** ranks beneficiaries based on need and eligibility criteria for optimal resource allocation.
- The DSS helps users understand which schemes they qualify for and how to maximize benefits, while factoring in key parameters like land size, crop type, income levels, and community needs.
- **Automated recommendations** generate scheme suggestions instantly based on real-time data integration, providing both **immediate eligibility status** and **long-term benefit projections**.

### **5. Multilingual Community Feedback Loop:**
- Upon registration, the **feedback system** is integrated throughout the platform, enabling continuous community engagement and voice-driven improvements.
- **Automated voice calls** reach tribal communities with limited digital access through local language phone calls (Hindi, Gondi, Santali, etc.).
- **Feedback collection** gathers community responses on scheme effectiveness, claim processing experiences, and needs assessment via IVR (Interactive Voice Response).
- **Continuous improvement** uses feedback to refine future schemes, improve service delivery, and update DSS algorithms dynamically.
- It's designed to be an inclusive engagement mechanism that ensures tribal voices shape policy and implementation.

### **6. AI + RAG-Powered Query System:**
- A **real-time AI assistant** designed to help users navigate the platform and extract insights from the centralized FRA repository instantly.
- The system has the ability to **process natural language queries** like "How many are eligible for PM-KISAN in Tripura?" and generate instant, data-backed responses.
- Users can ask questions, and the AI will retrieve relevant data, analyze patterns, and provide contextual answers with exportable reports.
- **Instant report generation** explores the centralized repository and generates exportable reports (PDF, Excel, shapefiles) without navigating the entire platform.
- **Context-aware responses** use RAG (Retrieval-Augmented Generation) to ensure answers are grounded in actual FRA data, not generic information.
- These reports serve as decision-support tools for district officers, state administrators, and policy researchers.

### **7. Comprehensive Analytics Dashboard:**
- **Key performance indicators** track claim processing rates, title recognition percentages, scheme disbursement, and beneficiary coverage in real-time.
- **Comparative analytics** show before/after metrics, state-wise performance, and trend analysis over time for data-driven insights.
- **Visual reporting** delivers interactive charts, heatmaps, and geospatial visualizations for data-driven decision-making.
- **Role-based access** provides different dashboard views for tribal communities, district officers, state authorities, and central monitoring agencies.

---

## **How It Works**:

1. **User Onboarding:**
   - Users register as **tribal claimants**, **village officers**, **district coordinators**, or **state administrators**.
   - **Hierarchical access** permissions are granted based on role—tribal members view their claims, officers manage village data, administrators oversee entire regions.

2. **Legacy Data Digitization:**
   - Scanned images of handwritten pattas, claims, and verification records are uploaded to the platform.
   - **OCR processing** using Tesseract.js and custom NER models extract structured data (names, plot numbers, coordinates, boundaries).
   - Extracted data is reviewed by human validators before final database entry through a **validation workflow**.

3. **Geospatial Visualization:**
   - Users navigate through **state → district → village → tribal group** to zoom into specific FRA areas on the interactive map.
   - **Boundary display** highlights approved FRA boundaries with color-coded status (individual rights, community rights).
   - Users can toggle **satellite overlay** to see actual terrain, forest cover, and land use patterns for verification.

4. **AI Asset Mapping:**
   - Platform fetches latest **satellite and SAR imagery** for FRA regions automatically.
   - **CNN analysis** through custom deep learning pipelines detects ponds, farms, vegetation types, and infrastructure.
   - The system generates **asset reports** with area measurements, GPS coordinates, and confidence scores for each detected resource.

5. **Decision Support & Scheme Mapping:**
   - The dashboard integrates FRA claim data with **DWLR water index**, **IoT agricultural sensors**, and **socio-economic surveys**.
   - **Eligibility calculation** evaluates each individual/community against scheme criteria (land size, crop type, income, etc.) using AI models.
   - **Recommendation generation** outputs personalized scheme lists ranked by relevance and potential benefit with application assistance.

6. **Community Feedback:**
   - System triggers automated phone calls in local languages to beneficiaries for continuous engagement.
   - **Voice response collection** records feedback via IVR for accessibility and reach.
   - **Sentiment analysis** processes feedback to identify satisfaction levels, common complaints, and improvement areas using AI.

7. **AI-Powered Querying:**
   - Users type or speak queries like "Show me rejected claims in Odisha from 2023" in natural language.
   - **RAG processing** retrieves relevant data from the centralized repository and generates contextual answers instantly.
   - Users can download results as formatted **PDFs, Excel sheets, or shapefiles** for GIS software without manual filtering.

---

## **Tech Stack**:

### **Frontend:**
- **Next.js**: Server-side rendering and static site generation for optimal performance and SEO.
- **TypeScript**: Type-safe development ensuring code reliability and maintainability.
- **Leaflet.js / Mapbox GL**: WebGIS visualization with layer controls, geofencing, and satellite imagery integration.
- **Recharts**: Data visualization library for analytics dashboards and comparative reports.

### **Backend:**
- **Node.js** & **Express.js**: RESTful APIs for authentication, claim management, asset retrieval, and DSS queries.
- **PostGIS**: Spatial database extension for PostgreSQL to store and query geospatial FRA data.
- **PostgreSQL**: Relational database for structured claim records, user profiles, and scheme mappings.

### **AI & Machine Learning:**
- **Tesseract.js + Custom NER**: OCR for digitizing handwritten documents with entity recognition for names, coordinates, and boundaries.
- **Custom CNN Models**: Built with TensorFlow/PyTorch for satellite image analysis and asset detection.
- **RAG Pipeline**: Combines LangChain, vector databases (Pinecone/FAISS), and LLMs (GPT-4/Gemini) for intelligent query responses.

---

## **Live Project:**
- [Visit VanAdhikar](https://dev-proto-1.vercel.app/)

---

## **Author**

- **Mouleeswaran**
- [GitHub Repository](https://github.com/MOULEESWARAN-25/VanAdhikar/)
