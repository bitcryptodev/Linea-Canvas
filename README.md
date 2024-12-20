# Linea-Canvas

**Linea-Canvas** is a decentralized platform that empowers users to collaboratively create vibrant pixel art on a 64x64 canvas. Participants can paint individual pixels or upload entire images, utilizing **PaintTokens**—an ERC20-based cryptocurrency—to purchase and set pixel colors. The system leverages smart contracts deployed on the **Linea Sepolia**  to manage token transactions and ensure secure, ownership-based modifications of the canvas. This seamless integration of blockchain technology fosters a community-driven art experience, allowing anyone to contribute to and own a piece of the collective masterpiece.

You can access the Dapp right now at [https://linea-canvas.vercel.app/](https://linea-canvas.vercel.app/)

![Violet and green simple art school logo](https://github.com/user-attachments/assets/ad6a4b3b-ec7f-4097-a497-058c1798f0ce)

## **Key Features**

- **64x64 Collaborative Canvas:** A fixed-size canvas where users can paint pixels individually or apply entire images.
- **PaintTokens (ERC20):** A cryptocurrency used to set pixel colors, ensuring secure and transparent transactions.
- **Smart Contract Integration:** Utilizes Solidity contracts deployed on Linea Sepolia.
- **Image Upload Capability:** Allows users to upload images, which can be applied to specific areas of the canvas by selecting designated regions.
- **User-Friendly Frontend:** An intuitive Next.js interface that facilitates easy interaction with the canvas, token purchases, and image uploads.

---

## **Technical Overview**

### **Smart Contracts**

- **Location:** `packages/hardhat/contracts/CollaborativeArtCanvas.sol` and `packages/hardhat/contracts/PaintToken.sol`


- **CollaborativeArtCanvas.sol:**
  - **Description:** Handles the canvas state, pixel color updates, and interactions with PaintTokens, enabling users to paint and own pixels securely.
  - **Deployment Address:** [0xD29e6E81BE21Fd453a0324053C3D5b0cED95958A](https://sepolia.lineascan.build/address/0xd29e6e81be21fd453a0324053c3d5b0ced95958a)

- **PaintToken.sol:**
  - **Description:** Manages the creation, distribution, and burning of PaintTokens, ensuring a controlled token economy within the platform.
  - **Deployment Address:** [0xfBE00f18773B1B2Cd37Bb09DE269C2A1F14868d7](https://sepolia.lineascan.build/address/0xfbe00f18773b1b2cd37bb09de269c2a1f14868d7)


## **Deployment Details**

- **Blockchain Network:** Linea Sepolia
- **Smart Contracts:**
  - **CollaborativeArtCanvas.sol**
    - **Address:** [0xD29e6E81BE21Fd453a0324053C3D5b0cED95958A](https://sepolia.lineascan.build/address/0xd29e6e81be21fd453a0324053c3d5b0ced95958a)
    - **Status:** Deployed and Verified

  - **PaintToken.sol**
    - **Address:** [0xfBE00f18773B1B2Cd37Bb09DE269C2A1F14868d7](https://sepolia.lineascan.build/address/0xfbe00f18773b1b2cd37bb09de269c2a1f14868d7)
    - **Status:** Deployed and Verified

## **Getting Started**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/bitcryptodev/Linea-Canvas
   cd Linea-Canvas
   ```

2. **Install Dependencies:**
   ```bash
   yarn install
   # or
   npm install
   ```

3. **Compile Smart Contracts:**
   ```bash
   cd packages/hardhat
   npx hardhat compile
   ```

4. **Deploy Contracts (If Not Already Deployed):**
   ```bash
   npx hardhat run scripts/deploy.js 
   ```

5. **Run the Frontend:**
   ```bash
   cd ../nextjs
   yarn dev
   # or
   npm run dev
   ```

6. **Access the Application:**
   - Open [http://localhost:3000](http://localhost:3000) in your browser to start painting!

---

## **Contributing**

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

---

## **License**

This project is licensed under the MIT License.

---

