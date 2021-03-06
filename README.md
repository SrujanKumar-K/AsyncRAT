# AsyncRAT
######### Extracting AsyncRAT configuration using CyberChef  ##########

![1](https://user-images.githubusercontent.com/71969773/166702465-45044769-1508-4dc1-9ad9-25fd68ef0840.PNG)![2](https://user-images.githubusercontent.com/71969773/166702492-21c5511a-b814-4108-80d5-6df0bd0f0f8f.PNG)




Steps to re-produce:
1. Open binary sample in dnSpy
2. Rightclick on loaded binary and select "Go to Entry Point"
3. Click on method "InitializeSettings()"
4. Click on variable "Key" and copy the entire the content and paste it to input section window of cyberchef

![image](https://user-images.githubusercontent.com/71969773/166680918-317b2016-0272-47d4-9ba5-249245c53160.png)

5. Inorder to extract the salt value, click on method "Aes256" and follow as per below snippet.

![image](https://user-images.githubusercontent.com/71969773/166681923-4344e2a0-5e25-4f57-aaeb-f16273d2f72e.png)


6. Please be ensure to select the proper  Salt text format while using the "Derive_PBKDF2_key"

![image](https://user-images.githubusercontent.com/71969773/166691893-10098296-808e-4ca2-8645-5df874be4600.png)

7. Similarly replicate  the same salt value at the end of Find_/_Replace

![image](https://user-images.githubusercontent.com/71969773/166692272-288c032a-f388-426e-9aab-4813cfa57791.png)
