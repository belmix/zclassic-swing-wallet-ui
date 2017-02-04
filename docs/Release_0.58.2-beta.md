# [ZClassic](http://zclassic.org) Desktop GUI Wallet - binary release v0.58.2-beta

This document describes how to install binary release v0.58.2-beta of the [ZClassic](http://zclassic.org) 
Desktop GUI Wallet. This release of the ZClassic Desktop GUI Wallet is tested with ZClassic version 
1.0.5. Users who encounter issues are welcome to report them in 
the [issues section](https://github.com/vaklinov/zclassic-swing-wallet-ui/issues). 

![Screenshot](https://github.com/vaklinov/zclassic-swing-wallet-ui/raw/master/docs/ZClassicWallet.png "Main Window")

## Installing and running the Wallet GUI

1. Downloading the wallet
 
   Download file [ZClassicSwingWalletUI.jar](https://github.com/vaklinov/zclassic-swing-wallet-ui/releases/download/0.58.2-beta/ZClassicSwingWalletUI.jar)
   and place it in a folder like `~/Downloads`. Then please make the JAR executable with a command like:
   ```
   user@ubuntu:~/Downloads$ chmod u+x ./ZClassicSwingWalletUI.jar
   ```
   
2. Verifying the download

   **This step is very important!** To verify that the file `ZClassicSwingWalletUI.jar` is an authentic release, you
   need to compute its SHA256 checksum, like this:
   ```
   user@ubuntu:~/Downloads$ sha256sum ZClassicSwingWalletUI.jar 
   eddfac69794f9319e7466d79c5f6dedca6fd90094f4e63417999006d23858e31  ZClassicSwingWalletUI.jar
   ```
   **If the resulting checksum is not `eddfac69794f9319e7466d79c5f6dedca6fd90094f4e63417999006d23858e31` then**
   **something is wrong and you should discard the downloaded wallet!**

3. Installing the downloaded ZClassic GUI wallet

  3.1. If you have built ZClassic from source code:

   Assuming you have already built from source code [ZClassic](http://zclassic.org) in directory `/home/user/zclassic/src` (for 
   example - this is the typical build dir. for ZClassic v1.0.5) which contains the command line tools `zcash-cli` 
   and `zcashd`, you need to take the file `ZClassicSwingWalletUI.jar` and copy it 
   to diretcory `/home/user/zclassic/src` (the same dir. that contains `zcash-cli` and `zcashd`). Example copy command:
   ```
   user@ubuntu:~/Downloads$ cp ./ZClassicSwingWalletUI.jar /home/user/zclassic/src    
   ```
   
4. Running the installed ZClassic GUI wallet

   Before running the GUI you need to start zcashd (e.g. `zcashd --daemon`). The wallet GUI is a Java program packaged 
   as an executable JAR file. It may be run from command line or started from another GUI tool (e.g. file manager). 
   Assuming you have already installed [ZClassic](http://zclassic.org) and the GUI Wallet `ZClassicSwingWalletUI.jar` in 
   directory `/home/user/zclassic/src` one way to run it from command line is:
   ```
   user@ubuntu:~$ java -jar /home/user/zclassic/src/ZClassicSwingWalletUI.jar
   ```
   If you are using Ubuntu (or similar ;) Linux you may instead just use the file manager and 
   right-click on the `ZClassicSwingWalletUI.jar` file and choose the option "Open with OpenJDK 8 Runtime". 
   This will start the ZClassic GUI wallet.

### Donations accepted
This project is non-commercial in nature and developed by volunteers. If you find the GUI
Wallet useful, please consider making a donation for its further development. Your contribution matters! Donations 
are accepted at ZClassic address:
```
zcaTKUNkohUgYj3C5bTapCKRk7JZapPfvCUj7GGBUWuBikx4sWEs5KSyd93b9jnjJnbDxnApyXyfeG482iJ5HzoC7cz6oob
```

### License
This program is distributed under an [MIT License](https://github.com/vaklinov/zclassic-swing-wallet-ui/raw/master/LICENSE).

### Disclaimer

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

