# base-gas-tracker
Track and log gas usage on Base using ethers.js.
import { ethers } from "ethers";


const provider = new ethers.JsonRpcProvider("https://mainnet.base.org");


async function getGas() {
const fee = await provider.getFeeData();
console.log(fee);
}


getGas();
