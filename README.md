# CloudFlare IP Scanner

CloudFlare IP Scanner is a program for scanning ASN IP addresses. The program allows you to find CloudFlare IP CDN and also determines the location and measures the latency of valid IP addresses.

![GUI](/img.png)

## Possibilities
- Scan IP addresses by ASN numbers
- TLS support
- Parallel query processing
- Saving results to a CSV file

## Installation

1. Install Go and set GOPATH.
2. Download the source code.
   ```sh
    git clone https://github.com/nxhack/CloudFlareIPScanner.git
    cd CloudFlareIPScanner
   ```

## Assembly

To compile the program, run the following command:

    go build -o CloudFlareIPScanner main.go

This will create an executable file CloudFlareIPScannerin the current directory.

## Usage

### Launch via command line

Run the program with the required arguments:

    ./CloudFlareIPScanner -asn <ASN > -port <порт> -max <мак> -tls <true/false>

Example:

    ./CloudFlareIPScanner -asn "AS13335,AS15169" -port 443 -max 50 -tls true

### Command line arguments

- asn: ASN numbers separated by commas (required).
- port: Port to scan (default 443).
- max: Maximum number of parallel requests (default 50), depends on internet speed.
- tls: Enable TLS (default true).

#### Contacts
Telegram https://t.me/bitcraken
