# Enhancing Predictive Performance on Long-Tail Trajectories via Clustering and Specialized Decoders

**Official repository for the paper**:  
**"Enhancing Predictive Performance on Long-Tail Trajectories via Clustering and Specialized Decoders"**  
📍 G. Ganeshaaraj, Tharindu Fernando, Sridha Sridharan, Clinton Fookes

## Abstract

Accurate forecasting of traffic participants’ future trajectories is crucial for the advancement of autonomous driving systems. However, current naturalistic datasets are imbalanced, with a dominance of simpler cases and scarcity of complex, rare (tail) scenarios. This imbalance challenges existing models, causing them to perform poorly in safety-critical tail conditions.

To tackle this, we propose a novel framework that leverages:
- **Embedding-based trajectory clustering**
- **A distribution-sensitive decoder module** tailored to head and tail samples
- **A trajectory clustering mechanism** for generating diverse and plausible predictions

Our method improves long-tail prediction performance by 19.5% (ADE) and 25.5% (FDE) on ETH/UCY datasets, while maintaining or exceeding state-of-the-art performance on head samples.

<p align="center">
  <img src="figures/tail.png" alt="Figure 1" width="600"/>
</p>

**Figure 1**: Distribution of sample difficulty on the ETH dataset with visual comparisons between our method and SOTA baselines on head and tail samples.

---

## 🧠 Model

<p align="center">
  <img src="figures/pipeline_v7.drawio.png" alt="Model Architecture" width="700"/>
</p>

**Figure 2**: Overview of our framework. It includes three stages:  
1. **Embedding Generation and Clustering** – to identify representative trajectory patterns  
2. **Fine-Tuning Decoders** – to adapt for tail samples  
3. **Inference with Trajectory Clustering** – to generate diverse and plausible multimodal predictions  

---

## 🧾 Code

Code is coming soon! Stay tuned 🔧🤖🔨

---

## 📊 Results

### 🟦 Head Sample Predictions  
<p float="left">
  <img src="figures/trajectory_visualization_112.pdf" width="200"/>
  <img src="figures/trajectory_visualization_1194.pdf" width="200"/>
  <img src="figures/trajectory_visualization_2531.pdf" width="200"/>
  <img src="figures/trajectory_visualization_34.pdf" width="200"/>
</p>

### 🟥 Tail Sample Predictions  
<p float="left">
  <img src="figures/trajectory_visualization_112.pdf" width="200"/>
  <img src="figures/trajectory_visualization_1194.pdf" width="200"/>
  <img src="figures/trajectory_visualization_2531.pdf" width="200"/>
  <img src="figures/trajectory_visualization_34.pdf" width="200"/>
</p>
