---

## 🧭 Layer Descriptions

### 🟦 Presentation Layer
- **Responsibilities**: Handles HTTP requests/responses.
- **Components**:
  - `Controller`: Receives client input and returns output.
  - `Dto`: Data Transfer Objects used in communication.
  - `Mapper`: Converts between DTOs and domain models.

### 🟨 Application Layer
- **Responsibilities**: Orchestrates business processes and application logic.
- **Components**:
  - `Usecase`: Executes specific operations or workflows.

### 🟩 Domain Layer
- **Responsibilities**: Contains business rules and logic.
- **Components**:
  - `Model`: Domain entities without external dependencies.
  - `Repository`: Interfaces abstracting persistence logic.

### 🟪 Infrastructure Layer
- **Responsibilities**: Provides concrete implementations for external concerns.
- **Components**:
  - `Entity`: JPA-annotated persistence classes.
  - `SpringDataRepository`: Interfaces extending Spring Data JPA repositories.
  - `JpaRepository`: Implements domain repositories using JPA.
  - `Mapper`: Converts between persistence entities and domain models.

---
