# AvatarCLIP Project

## Overview
AvatarCLIP is a multimodal AI framework designed to generate avatars based on textual prompts. This guide provides a detailed explanation of the steps followed to set up, execute, and validate the AvatarCLIP model. 

---

<h4 align="center">
  <a href="https://colab.research.google.com/drive/1js37DAVus060jlSfWE2hYcDs_HOPhrkI?usp=sharing#scrollTo=AWs9vh1FJzXP" target='_blank'>[Colab Demo]</a>
</h4>

## Prerequisites Required

1. **Local Environment:**
   - Operating System: Windows or Linux.
   - Required Software:
     - Python 3.8 or above.
     - PyTorch.
     - CUDA toolkit (for GPU acceleration).
     - Microsoft Visual Studio Build Tools (for Windows users).

2. **Cloud Environment:**
   - Google Colab account.
   - Preconfigured GPU environment access.

---

## Setup Steps

### 1. Local Environment Setup

1. Install the following:
   - Python 3.8+.
   - PyTorch (version compatible with your CUDA toolkit).
   - CUDA toolkit and Microsoft Visual Studio Build Tools (Windows).

2. Clone the AvatarCLIP repository:
   ```bash
   git clone https://github.com/hongfz16/AvatarCLIP.git
   cd AvatarCLIP
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Test the environment by running sample scripts.
   - Use CUDA 12.6 with Build Tools 2022.
   - If issues arise, downgrade to CUDA 11.3 with Build Tools 2019.

### 2. Cloud Environment Setup (Google Colab)

1. Open Google Colab and create a new notebook.
2. Clone the AvatarCLIP repository:
   ```python
   !git clone https://github.com/hongfz16/AvatarCLIP.git
   ```
3. Navigate to the repository:
   ```python
   %cd AvatarCLIP
   ```
4. Install dependencies:
   ```python
   !pip install -r requirements.txt
   ```
5. Upgrade PyTorch and CUDA (if needed):
   ```python
   !pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
   ```

---

## Execution Steps

### 1. Input Preparation

- Prepare a textual prompt. For example, input the prompt:
  ```
  "Iron Man"
  ```

### 2. Model Execution

1. Run the model to process the input prompt and generate an avatar.
   - For Colab:
     ```python
     !python generate_avatar.py --input "Iron Man"
     ```

2. Wait for the model to complete the generation process.
3. The output avatar will be saved in the output directory.

---

## Key Challenges

1. **Compatibility Issues:**
   - PyTorch and CUDA versions often conflicted, causing errors during setup.
   - Resolved by upgrading or downgrading dependencies iteratively.

2. **Cloud Computing Limits:**
   - Google Colab’s GPU resources limited the model to generate only static avatars.

3. **Initial Dependency Errors in Colab:**
   - Resolved by ensuring all dependencies matched the preconfigured environment.

---

## Results

- Successfully generated a static “Iron Man” avatar using Google Colab.
- Demonstrated the potential of AvatarCLIP for multimodal avatar generation.

---

## Future Directions

1. **Enhanced Computational Power:**
   - Explore high-performance GPU cloud services like AWS or Azure.
2. **Animated Outputs:**
   - Extend capabilities to generate dynamic, animated avatars.
3. **User Interface Development:**
   - Create an intuitive front-end interface for broader accessibility.

---

## Notes
- For advanced features, consult the AvatarCLIP GitHub documentation.
- Ensure that all dependencies are updated before starting the process.
