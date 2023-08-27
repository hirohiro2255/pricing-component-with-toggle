```mermaid
flowchart TD
A[page.svelte] --> |isMonthly: boolean| B[Layout]
B --> |isMonthly| C[CardList]
B --> |isMonthly| D[Header]
```
