# webcam-recon

Some Syntax examples:
nmap --script-help AXISwebcam-recon.nse
nmap -sV -Pn -p 80-86,92,8080-8082 --open --script AXISwebcam-recon.nse 216.99.115.136
nmap -sV -Pn -p 80-86,92,8080-8082 --open --script AXISwebcam-recon.nse --script-args "uri=/view/viewer_index.shtml" 217.78.137.43
nmap -sS -Pn -p 80-86,92,8080-8082 --script AXISwebcam-recon.nse --script-args "agent=Mozilla/5.0 (compatible; EvilMonkey)" 50.93.227.204
nmap -sS -Pn -p 80,8080-8082 --open --script AXISwebcam-recon.nse --script-args "agent=Mozilla/5.0 (compatible),uri=/fd" 194.150.15.187
nmap -sS -v -Pn -n -T5 -iR 500 -p 8080-8086 --open --script=http-headers.nse,AXISwebcam-recon.nse -D 65.49.82.3 -oN webcam_reports.txt
