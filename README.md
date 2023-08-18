# ALEO.DEPLOY.SMART.CONTRACT
How to deploy smart contract  on Aleo


🚀🧨


Install prerequisites
------------------------------------------------------------------
First run this👇code

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

rustup install stable

rustup update stable

rustup default stable

git clone https://github.com/AleoHQ/leo
cd leo

apt install clang gcc libssl-dev pkg-config

cargo install --path .

git clone https://github.com/AleoHQ/snarkOS.git --depth 1
cd snarkOS

./build_ubuntu.sh

cargo install --path

(receive a fauucet)
------------------------------------------------------------------
Send this text👇
Send 50 credits to
 your wallet address
To number
+18678885688
------------------------------------------------------------------
Now run this code👇

cd $HOME

mkdir demo_deploy_Leo_app && cd demo_deploy_Leo_app

WALLETADDRESS=""

APPNAME=helloworld_"${WALLETADDRESS:4:6}"

leo new "${APPNAME}"

PATHTOAPP=$(realpath -q $APPNAME)

cd $PATHTOAPP && cd ..

PRIVATEKEY=""

RECORD=""

snarkos developer deploy "${APPNAME}.aleo" --private-key "${PRIVATEKEY}" --query "https://vm.aleo.org/api" --path "./${APPNAME}/build/" --broadcast "https://vm.aleo.org/api/testnet3/transaction/broadcast" --fee 600000 --record "${RECORD}"


۰(۰۰(Copy the last three lines and paste them in the appropriate place in the form)۰۰)۰


FINISH
ALEO🎖️
