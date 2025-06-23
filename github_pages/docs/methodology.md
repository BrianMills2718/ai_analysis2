# Analysis Methodology

## Data Collection

### Source Data
- **RAND Corporation GraphQL API** - 48,876+ publications with full metadata
- **Document Database** - 9,116 documents with 564K text chunks
- **FAISS Vector Index** - 563K embeddings for semantic search

### Time Period
- **Focus:** 2020-2025 (Enhanced Modern Era)
- **Documents:** 2,230 publications with perfect API coverage
- **Quality Control:** 100% year data validation and cleaning

## Processing Pipeline

### 1. Document Analysis
- **LLM Processing:** Gemini 2.5 Flash for methodology extraction
- **Success Rate:** 100% completion across all documents
- **Method Detection:** Pattern-based identification of research approaches
- **AI Technology Detection:** Automated identification of AI tools and methods

### 2. Organizational Mapping
- **Division Detection:** High-confidence pattern matching
- **Coverage:** 28.2% with strict quality controls ("low coverage > bad coverage")
- **FFRDCs:** Project AIR FORCE, NDRI, Arroyo Center, HSOAC
- **Methods Centers:** RAND Forecasting Initiative, TASP, CRC, etc.

### 3. Topic Extraction
- **Source:** RAND API taxonomy and taxonomy_terms fields
- **Coverage:** 99.3% (2,215/2,230 documents)
- **Categories:** 892 unique topics across research domains
- **Processing:** Memory-safe streaming to handle 324MB metadata file

### 4. Relationship Mapping
- **Total Relationships:** 98,688 mapped connections
- **Dimensions:** Methods ↔ AI ↔ Divisions ↔ Authors ↔ Time ↔ Topics
- **Data Model:** Relational structure with 13 tables and cross-references

## Quality Assurance

### Data Validation
- **Memory Management:** Streaming approaches for large files (324MB → 5.3MB processing)
- **Pattern Validation:** High-confidence organizational boundaries only
- **Temporal Accuracy:** Perfect year coverage for 2020+ period
- **Author Coverage:** 78.7% with verified email addresses

### Methodology Rigor
- **No Analysis Bias:** Raw numbers and breakdowns only
- **Reproducible Process:** All scripts and transformations documented
- **Error Handling:** Comprehensive validation at each processing stage
- **Performance Optimization:** Web-ready data structures

## Dashboard Implementation

### Architecture
- **Frontend:** Pure JavaScript with real-time filtering
- **Data Model:** Document-centric with dimensional lookups
- **Performance:** Client-side processing for instant responses
- **Export:** JSON download functionality for further analysis

### Filter Capabilities
- **Multi-dimensional:** Any combination of 6 filter dimensions
- **Real-time:** Instant statistics and result updates
- **Scalable:** Handles 2,230+ documents with sub-second response

## Limitations

### Known Constraints
- **Topic Data:** Limited to RAND API taxonomy (no custom classification)
- **Division Coverage:** Conservative approach results in 28.2% coverage
- **Display Limits:** Web interface shows top 50-100 results for performance
- **Memory Constraints:** Large JSON files require streaming approaches

### Future Enhancements
- **Extended Topic Analysis:** Custom research area classification
- **Enhanced Collaboration Networks:** Author relationship mapping  
- **Temporal Trend Analysis:** Statistical significance testing
- **Advanced Visualizations:** Network graphs and interactive charts
