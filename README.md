# nuclei-templates
nuclei templete for fuzzing 


How to Use
1. Select Domain or subdomain by using -u path for fuzzing 
2. Add the template path by -t 

Example:-
nuclei -u https://www.tesla.com -t /root/nuclei-templates/exposures/files/hiddenfile.yaml

It will give you all posiible hidden files that i added on my template you can add more hidden words to get more possibilities. 
