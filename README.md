# README.
"Eliminating high freelancer fees with Polkadot: A non-custodial marketplace for secure, instant gig settlements via native USDT/USDC."
# Clone the repository
git clone https://github.com/[PolkaGig]/[PolkaGig].git

# Navigate to contracts
cd contracts
cargo contract build

# Start the frontend
cd ../frontend
npm install
npm run dev


​1. The Onboarding Flow (Top Section)
​Step: User signs up via Social Login (Google/X).
​Action: Your app uses a Proxy Account (specifically a StakingOperator-style restricted proxy).
​Visual: A dashed line from the "User" to a "Hidden Polkadot Address."
​Note: This tells voters: "Users don't need to manage seed phrases immediately."
​2. The Job & Escrow Flow (Middle Section)
​Step: Employer posts a job and deposits USDT/USDC.
​Action: The app triggers an ink! Smart Contract on Asset Hub.
​Visual: An arrow labeled "Deposit Stablecoin" moving from the Employer’s wallet to the "Escrow Contract" box on Asset Hub.
​Mechanism: Mention "XCM v5" here. It shows you're using the latest 2026 tech to handle cross-chain fees efficiently.
​3. The Work & Payout Flow (Bottom Section)
​Step: Freelancer submits work; Employer clicks "Approve."
​Action: The Escrow Contract releases USDT to the Freelancer.
​Simultaneous Action: A "Success Signal" is sent to the People Chain.
​Visual: Two arrows branching out from the Escrow Contract:
​One to the Freelancer (labeled "Instant Payout").
​One to the People Chain (labeled "Mint Reputation Attestation").
