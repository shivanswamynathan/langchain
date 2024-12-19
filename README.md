# Temperature 
Temperature controls the randomness of the model's output, affecting how creative or focused it is.

## Range
`0` to `1` (commonly used values; higher values like `1.5` are also possible in some models).

- **Temperature = 0**:
  - The model becomes highly deterministic.
  - It always picks the most probable response, leading to more predictable and factual outputs.
  - Best for tasks requiring precision (e.g., math, coding).

- **Temperature = 1**:
  - The model becomes more creative and random.
  - It considers a wider range of possible responses, leading to more diverse and imaginative outputs.
  - Useful for creative writing or generating multiple perspectives.

---

# Prompt Template
A prompt template is a structured format that guides the model on how to generate a response.

## Why use it?
- To standardize input to the model.
- To include necessary context or instructions.

### Example
- **Template**: `"Translate the following text to French: {input_text}"`
- **Input**: `"Hello, how are you?"`
- **What the model sees**: `"Translate the following text to French: Hello, how are you?"`

---

# Chains

Chains are sequences of tasks/models that work together to complete complex workflows.

## Why do we need them?
- Many tasks involve multiple steps.
- Chains allow combining models and logic to handle these steps efficiently.

### Types of Chains

#### Sequential Chain
- Tasks happen one after the other.
- Output of one step becomes input to the next.
- **Example**: Summarize a text → Translate it into another language.

#### Combine Chain
- Integrates multiple inputs or models.
- Combines outputs from different steps/models into a single result.
- **Example**: A chain that collects data from multiple documents and creates a unified summary.

---

# Simple Sequential Chain vs Sequential Chain

### Simple Sequential Chain
- Linear flow: Task A → Task B → Task C.
- No branching or additional logic.
- Suitable for straightforward tasks.

### Sequential Chain
- More advanced, may include conditional logic.
- Tasks can depend on specific conditions or inputs.
- **Example**: Based on the user's input, decide which task to perform next.
