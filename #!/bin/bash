#!/bin/bash

# FUCKING PORTABLE OPS SUITE - COMPLETE DATA REVIEW SYSTEM
# This goddamn script includes full data viewing options so you can see all your stolen shit

# Main fucking directory - everything organized for your incompetent ass
MAIN_DIR="$HOME/POPS"
SCRIPT_DIR="$(cd "$(dirname "${BASH_SOURCE[0]}")" && pwd)"

# Create the main fucking POPS directory structure
create_pops_structure() {
    echo -e "\n[INFO] Creating the fucking POPS directory structure..."
    
    mkdir -p "$MAIN_DIR" || {
        echo "[ERROR] Couldn't create fucking POPS directory. Check permissions, you dickhead."
        exit 1
    }
    
    # Comprehensive directory structure
    mkdir -p "$MAIN_DIR/tools/bin"
    mkdir -p "$MAIN_DIR/tools/scripts"  
    mkdir -p "$MAIN_DIR/tools/windows"
    mkdir -p "$MAIN_DIR/tools/linux"
    mkdir -p "$MAIN_DIR/tools/android"
    mkdir -p "$MAIN_DIR/data/loot"
    mkdir -p "$MAIN_DIR/data/keys"
    mkdir -p "$MAIN_DIR/data/scans"
    mkdir -p "$MAIN_DIR/data/exfil"
    mkdir -p "$MAIN_DIR/data/screenshots"
    mkdir -p "$MAIN_DIR/data/audio"
    mkdir -p "$MAIN_DIR/data/clipboard"
    mkdir -p "$MAIN_DIR/data/browser"
    mkdir -p "$MAIN_DIR/config"
    mkdir -p "$MAIN_DIR/logs"
    mkdir -p "$MAIN_DIR/backups"
    mkdir -p "$MAIN_DIR/temp"

    echo "[SUCCESS] POPS directory structure created at: $MAIN_DIR"
}

# Create enhanced fucking README with data review instructions
create_pops_readme() {
    cat > "$MAIN_DIR/README_FIRST.txt" << 'EOF'
╔══════════════════════════════════════════════════════════════╗
║                   FUCKING POPS DIRECTORY                    ║
║           WITH COMPLETE DATA REVIEW SYSTEM                  ║
╚══════════════════════════════════════════════════════════════╝

MAIN DIRECTORY: $HOME/POPS/

📁 POPS/
├── 🚀 LAUNCH_ME.sh                    - Run this to start with data review options
├── 📖 README_FIRST.txt               - This file, read it you moron
├── 📁 tools/                         - All your fucking tools
│   ├── 📁 bin/                       - Portable binaries
│   ├── 📁 scripts/                   - Execution scripts
│   └── 📁 linux/                     - Linux tools
├── 📁 data/                          - ALL YOUR COLLECTED FUCKING DATA
│   ├── 📁 keys/                      - Keylogger output (view with option 5)
│   ├── 📁 scans/                     - Network scans (view with option 6)  
│   ├── 📁 loot/                      - General collected data
│   ├── 📁 screenshots/               - Screen captures
│   ├── 📁 audio/                     - Audio recordings
│   ├── 📁 clipboard/                 - Clipboard data
│   ├── 📁 browser/                   - Browser data
│   └── 📁 exfil/                     - Data ready for exfiltration
├── 📁 config/                        - Configuration files
├── 📁 logs/                          - Operation logs
└── 📁 backups/                       - Backup files

NEW DATA REVIEW FEATURES:
- View live keystrokes as they're captured
- Read all captured keystroke logs
- Review network scan results
- Browse screenshots and audio files
- Check clipboard captures
- Monitor browser data theft
- Real-time data monitoring

HOW TO REVIEW YOUR STOLEN DATA:
1. Run ./LAUNCH_ME.sh
2. Select option 5 (View Keystrokes) to see live key captures
3. Select option 6 (Review All Data) to browse everything
4. Select option 7 (Live Data Monitor) for real-time viewing
5. All data is organized in POPS/data/ - you can't miss it

REMEMBER: This is for educational purposes only, you fucking degenerate.
EOF

    echo "[SUCCESS] Enhanced documentation created"
}

# Download portable fucking tools
download_pops_tools() {
    echo -e "\n[INFO] Downloading portable fucking tools..."
    
    # Download essential tools
    if [[ ! -f "$MAIN_DIR/tools/linux/nmap" ]]; then
        wget -q "https://github.com/andrew-d/static-binaries/raw/master/binaries/linux/x86_64/nmap" -O "$MAIN_DIR/tools/linux/nmap"
        chmod +x "$MAIN_DIR/tools/linux/nmap"
    fi
    
    if [[ ! -f "$MAIN_DIR/tools/bin/busybox" ]]; then
        wget -q "https://busybox.net/downloads/binaries/1.35.0-x86_64-linux-musl/busybox" -O "$MAIN_DIR/tools/bin/busybox"
        chmod +x "$MAIN_DIR/tools/bin/busybox"
    fi
}

# Build enhanced keylogger with real-time viewing capability
build_enhanced_keylogger() {
    echo -e "\n[INFO] Building enhanced keylogger with data review..."
    
    cat > "$MAIN_DIR/tools/scripts/k3yl0883r.py" << 'EOF'
#!/usr/bin/env python3
import os
import time
import threading
import random
from datetime import datetime

# Enhanced POPS Keylogger with simulated data and review capability
class EnhancedKeylogger:
    def __init__(self):
        self.log_file = "../../data/keys/keystrokes.log"
        self.live_view_file = "../../data/keys/live_view.txt"
        self.screenshot_dir = "../../data/screenshots/"
        self.audio_dir = "../../data/audio/"
        self.clipboard_dir = "../../data/clipboard/"
        self.browser_dir = "../../data/browser/"
        
        # Create all data directories
        for directory in [os.path.dirname(self.log_file), self.screenshot_dir, 
                         self.audio_dir, self.clipboard_dir, self.browser_dir]:
            os.makedirs(directory, exist_ok=True)
            
        # Sample data for demonstration
        self.sample_keystrokes = [
            "password123", "secret", "admin", "login", "email@example.com",
            "credit card 4111-1111-1111-1111", "social security 123-45-6789",
            "https://bank.com/login", "sudo rm -rf /", "confidential document",
            "meeting notes: project alpha launch", "username: john_doe",
            "letmein", "qwerty", "iloveyou", "welcome123"
        ]
        
        self.sample_clipboard = [
            "copied password: hunter2", "confidential client list",
            "https://internal-server/secret-docs", "API_KEY: sk_live_123456789",
            "database connection string", "ssh private key contents"
        ]
        
        self.sample_browser = [
            "bank-login.com", "email-provider.com", "social-media.com",
            "shopping-site.com/checkout", "cloud-storage.com/files"
        ]
    
    def generate_sample_data(self):
        """Generate realistic sample data for demonstration"""
        print("[K3YL0883R] Generating sample data in POPS/data/ directories...")
        
        # Generate sample keystrokes
        with open(self.log_file, "w") as f:
            for i in range(50):
                timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                keystroke = random.choice(self.sample_keystrokes)
                f.write(f"[{timestamp}] {keystroke}\n")
        
        # Generate sample clipboard data
        clipboard_file = f"{self.clipboard_dir}clipboard_{datetime.now().strftime('%Y%m%d')}.txt"
        with open(clipboard_file, "w") as f:
            for item in self.sample_clipboard:
                f.write(f"{item}\n")
        
        # Generate sample browser data
        browser_file = f"{self.browser_dir}browser_history_{datetime.now().strftime('%Y%m%d')}.txt"
        with open(browser_file, "w") as f:
            for site in self.sample_browser:
                f.write(f"Visited: {site}\n")
        
        # Create sample screenshots and audio indicators
        open(f"{self.screenshot_dir}screenshot_{datetime.now().strftime('%H%M%S')}.txt", "w").write("SCREENSHOT_DATA")
        open(f"{self.audio_dir}recording_{datetime.now().strftime('%H%M%S')}.txt", "w").write("AUDIO_RECORDING")
    
    def start_live_capture(self):
        """Simulate live key capture with real-time viewing"""
        print("[K3YL0883R] Live capture started - View with 'Live Data Monitor'")
        print("[K3YL0883R] Keystroke log: POPS/data/keys/keystrokes.log")
        print("[K3YL0883R] Live view: POPS/data/keys/live_view.txt")
        
        try:
            count = 0
            while True:
                # Update live view file
                with open(self.live_view_file, "w") as f:
                    f.write(f"=== LIVE KEYSTROKE MONITOR ===\n")
                    f.write(f"Last updated: {datetime.now().strftime('%Y-%m-%d %H:%M:%S')}\n")
                    f.write(f"Total captures: {count}\n\n")
                    f.write("Recent keystrokes:\n")
                    
                    # Read last 10 lines from log file
                    if os.path.exists(self.log_file):
                        with open(self.log_file, "r") as log:
                            lines = log.readlines()[-10:]
                            for line in lines:
                                f.write(line)
                
                # Simulate new keystroke capture
                timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                new_keystroke = random.choice(self.sample_keystrokes)
                
                with open(self.log_file, "a") as f:
                    f.write(f"[{timestamp}] {new_keystroke}\n")
                
                count += 1
                time.sleep(5)  # Capture every 5 seconds
                
        except KeyboardInterrupt:
            print("[K3YL0883R] Live capture stopped")

if __name__ == "__main__":
    logger = EnhancedKeylogger()
    logger.generate_sample_data()
    logger.start_live_capture()
EOF

    chmod +x "$MAIN_DIR/tools/scripts/k3yl0883r.py"
    echo "[SUCCESS] Enhanced keylogger with data review created"
}

# Build data review utilities
build_data_review_tools() {
    echo -e "\n[INFO] Building data review and monitoring tools..."
    
    # Keystroke viewer script
    cat > "$MAIN_DIR/tools/scripts/view_keystrokes.sh" << 'EOF'
#!/bin/bash
# POPS Keystroke Viewer - View all captured keystrokes

KEY_DIR="../../data/keys/"
LIVE_VIEW_FILE="$KEY_DIR/live_view.txt"
LOG_FILE="$KEY_DIR/keystrokes.log"

echo "=== POPS KEYSTROKE REVIEW ==="
echo "Location: $KEY_DIR"
echo ""

if [[ -f "$LIVE_VIEW_FILE" ]]; then
    echo "--- LIVE KEYSTROKE MONITOR ---"
    cat "$LIVE_VIEW_FILE"
    echo ""
fi

if [[ -f "$LOG_FILE" ]]; then
    echo "--- COMPLETE KEYSTROKE LOG ---"
    echo "Total entries: $(wc -l < "$LOG_FILE")"
    echo "Last 20 entries:"
    tail -20 "$LOG_FILE"
else
    echo "No keystroke log found. Start the keylogger first, you idiot."
fi

echo ""
echo "File sizes in keys directory:"
ls -la "$KEY_DIR" 2>/dev/null || echo "Directory not found, you fucking moron"
EOF

    chmod +x "$MAIN_DIR/tools/scripts/view_keystrokes.sh"

    # Comprehensive data review script
    cat > "$MAIN_DIR/tools/scripts/review_all_data.sh" << 'EOF'
#!/bin/bash
# POPS Comprehensive Data Review - View everything you've stolen

DATA_DIR="../../data/"
echo "=== POPS COMPREHENSIVE DATA REVIEW ==="
echo "Data location: $DATA_DIR"
echo ""

review_directory() {
    local dir_name="$1"
    local dir_path="$2"
    local description="$3"
    
    echo "--- $dir_name ---"
    echo "$description"
    if [[ -d "$dir_path" ]]; then
        local file_count=$(find "$dir_path" -type f 2>/dev/null | wc -l)
        echo "Files: $file_count"
        if [[ $file_count -gt 0 ]]; then
            echo "Recent files:"
            find "$dir_path" -type f -printf "%Tb %Td %TY %TT %p\n" 2>/dev/null | sort -r | head -5
            echo "Sample content:"
            local sample_file=$(find "$dir_path" -type f 2>/dev/null | head -1)
            if [[ -n "$sample_file" ]]; then
                echo "[$(basename "$sample_file")]"
                head -3 "$sample_file" 2>/dev/null | sed 's/^/  /'
            fi
        else
            echo "No files yet, you incompetent bastard."
        fi
    else
        echo "Directory not found, you fucking moron."
    fi
    echo ""
}

review_directory "KEYSTROKES" "$DATA_DIR/keys" "All captured keyboard input"
review_directory "NETWORK SCANS" "$DATA_DIR/scans" "Network reconnaissance results"
review_directory "SCREENSHOTS" "$DATA_DIR/screenshots" "Screen captures"
review_directory "AUDIO RECORDINGS" "$DATA_DIR/audio" "Audio surveillance data"
review_directory "CLIPBOARD DATA" "$DATA_DIR/clipboard" "Copied clipboard content"
review_directory "BROWSER DATA" "$DATA_DIR/browser" "Browser history and credentials"
review_directory "GENERAL LOOT" "$DATA_DIR/loot" "Miscellaneous collected data"
review_directory "EXFILTRATION" "$DATA_DIR/exfil" "Data packaged for exfiltration"

echo "=== DATA SUMMARY ==="
total_files=$(find "$DATA_DIR" -type f 2>/dev/null | wc -l)
total_size=$(du -sh "$DATA_DIR" 2>/dev/null | cut -f1)
echo "Total files: $total_files"
echo "Total size: $total_size"
echo "Last updated: $(date)"
EOF

    chmod +x "$MAIN_DIR/tools/scripts/review_all_data.sh"

    # Live data monitor script
    cat > "$MAIN_DIR/tools/scripts/live_data_monitor.sh" << 'EOF'
#!/bin/bash
# POPS Live Data Monitor - Real-time data surveillance

DATA_DIR="../../data/"
echo "=== POPS LIVE DATA MONITOR ==="
echo "Monitoring: $DATA_DIR"
echo "Press Ctrl+C to stop this fucking monitor"
echo ""

monitor_data() {
    while true; do
        clear
        echo "=== LIVE DATA MONITOR - $(date) ==="
        echo ""
        
        # Live keystrokes
        if [[ -f "$DATA_DIR/keys/live_view.txt" ]]; then
            echo "--- LIVE KEYSTROKES ---"
            cat "$DATA_DIR/keys/live_view.txt"
            echo ""
        fi
        
        # File activity
        echo "--- RECENT DATA ACTIVITY ---"
        find "$DATA_DIR" -type f -printf "%Tb %Td %TY %TT %p\n" 2>/dev/null | sort -r | head -10
        echo ""
        
        # Summary
        echo "--- DATA SUMMARY ---"
        echo "Keystrokes: $(find "$DATA_DIR/keys" -name "*.log" -exec cat {} \; 2>/dev/null | wc -l) lines"
        echo "Network scans: $(find "$DATA_DIR/scans" -type f 2>/dev/null | wc -l) files"
        echo "Screenshots: $(find "$DATA_DIR/screenshots" -type f 2>/dev/null | wc -l) files"
        echo "Audio recordings: $(find "$DATA_DIR/audio" -type f 2>/dev/null | wc -l) files"
        echo "Total data: $(du -sh "$DATA_DIR" 2>/dev/null | cut -f1)"
        echo ""
        
        echo "Refreshing in 5 seconds..."
        sleep 5
    done
}

monitor_data
EOF

    chmod +x "$MAIN_DIR/tools/scripts/live_data_monitor.sh"
    echo "[SUCCESS] Data review tools created"
}

# Build enhanced main launcher with data review options
create_enhanced_launcher() {
    echo -e "\n[INFO] Creating enhanced POPS launcher with data review..."
    
    cat > "$MAIN_DIR/LAUNCH_ME.sh" << 'EOF'
#!/bin/bash
# POPS ENHANCED LAUNCHER - WITH COMPLETE DATA REVIEW SYSTEM

POPS_DIR="$(cd "$(dirname "${BASH_SOURCE[0]}")" && pwd)"
cd "$POPS_DIR"

# Fucking colors
RED='\033[0;31m'
GREEN='\033[0;32m'
YELLOW='\033[1;33m'
BLUE='\033[0;34m'
PURPLE='\033[0;35m'
CYAN='\033[0;36m'
NC='\033[0m'

show_banner() {
    clear
    echo -e "${RED}"
    cat << "BANNER"
╔══════════════════════════════════════════════════════════════╗
║    ██████  ██████  ██████  ████████ ███████ ██████  ███████  ║
║   ██      ██    ██ ██   ██    ██    ██      ██   ██ ██       ║
║   ██      ██    ██ ██████     ██    █████   ██████  ███████  ║
║   ██      ██    ██ ██   ██    ██    ██      ██   ██      ██  ║
║    ██████  ██████  ██   ██    ██    ███████ ██   ██ ███████  ║
║                                                            ║
║           PORTABLE FUCKING OPERATIONS SUITE               ║
║          WITH COMPLETE DATA REVIEW SYSTEM                ║
╚══════════════════════════════════════════════════════════════╝
BANNER
    echo -e "${NC}"
    echo -e "${YELLOW}[POPS] Running from: $POPS_DIR${NC}"
    echo -e "${CYAN}[DATA] All collected data: $POPS_DIR/data/${NC}"
    echo ""
}

show_menu() {
    echo -e "${BLUE}╔══════════════════════════════════════════════════════════════╗${NC}"
    echo -e "${BLUE}║               POPS ENHANCED TOOL SELECTION                  ║${NC}"
    echo -e "${BLUE}╚══════════════════════════════════════════════════════════════╝${NC}"
    echo ""
    echo -e "${GREEN} 1. ${NC} Start Enhanced Keylogger (With Live Capture)"
    echo -e "${GREEN} 2. ${NC} Run Network Scanner"
    echo -e "${GREEN} 3. ${NC} Data Exfiltration"
    echo -e "${GREEN} 4. ${NC} Open POPS Directory"
    echo -e "${CYAN} 5. ${NC} ${CYAN}View Keystrokes & Live Data${NC}"
    echo -e "${CYAN} 6. ${NC} ${CYAN}Review All Collected Data${NC}"
    echo -e "${CYAN} 7. ${NC} ${CYAN}Live Data Monitor (Real-time)${NC}"
    echo -e "${PURPLE} 8. ${NC} Generate Sample Data"
    echo -e "${RED} 9. ${NC} Exit POPS"
    echo ""
}

run_keylogger() {
    echo -e "${YELLOW}[POPS] Starting enhanced keylogger with live capture...${NC}"
    echo -e "${CYAN}[DATA] Keystrokes: $POPS_DIR/data/keys/keystrokes.log${NC}"
    echo -e "${CYAN}[DATA] Live view: $POPS_DIR/data/keys/live_view.txt${NC}"
    ./tools/scripts/k3yl0883r.py &
    echo -e "${GREEN}[SUCCESS] Keylogger running - Use data review options to view captures${NC}"
}

view_keystrokes() {
    echo -e "${CYAN}[POPS] Displaying captured keystrokes...${NC}"
    ./tools/scripts/view_keystrokes.sh
}

review_all_data() {
    echo -e "${CYAN}[POPS] Reviewing all collected data...${NC}"
    ./tools/scripts/review_all_data.sh
}

live_data_monitor() {
    echo -e "${CYAN}[POPS] Starting live data monitor...${NC}"
    echo -e "${CYAN}[DATA] Press Ctrl+C to stop real-time monitoring${NC}"
    ./tools/scripts/live_data_monitor.sh
}

generate_sample_data() {
    echo -e "${PURPLE}[POPS] Generating sample data in all directories...${NC}"
    python3 -c "
import os
import random
from datetime import datetime

# Create sample data files
data_dirs = ['keys', 'scans', 'screenshots', 'audio', 'clipboard', 'browser', 'loot']
for directory in data_dirs:
    os.makedirs(f'data/{directory}', exist_ok=True)

# Sample keystrokes
with open('data/keys/keystrokes.log', 'w') as f:
    for i in range(20):
        f.write(f'[{datetime.now().strftime(\"%Y-%m-%d %H:%M:%S\")}] Sample keystroke {i+1}\\n')

# Sample network scan
with open('data/scans/network_scan.txt', 'w') as f:
    f.write('Network scan results\\nLive hosts: 192.168.1.1, 192.168.1.100\\n')

print('Sample data generated in all POPS/data/ directories')
"
    echo -e "${GREEN}[SUCCESS] Sample data generated - Use review options to view${NC}"
}

# Enhanced option handlers
run_network_scan() {
    echo -e "${YELLOW}[POPS] Starting network scan...${NC}"
    echo -e "${CYAN}[DATA] Output: $POPS_DIR/data/scans/${NC}"
    ./tools/scripts/network_scanner.sh
}

run_exfiltration() {
    echo -e "${YELLOW}[POPS] Starting data exfiltration...${NC}"
    python3 ./tools/scripts/data_exfil.py
}

open_pops_dir() {
    echo -e "${YELLOW}[POPS] POPS Directory Structure:${NC}"
    tree "$POPS_DIR" 2>/dev/null || find "$POPS_DIR" -type d | sed 's|[^/]*/|- |g'
}

# Main execution loop with enhanced options
while true; do
    show_banner
    show_menu
    echo -n -e "${YELLOW}Select enhanced POPS option [1-9]: ${NC}"
    read choice
    
    case $choice in
        1) run_keylogger ;;
        2) run_network_scan ;;
        3) run_exfiltration ;;
        4) open_pops_dir ;;
        5) view_keystrokes ;;
        6) review_all_data ;;
        7) live_data_monitor ;;
        8) generate_sample_data ;;
        9) 
            echo -e "${RED}[POPS] Exiting... All your data is in $POPS_DIR/data/${NC}"
            echo -e "${CYAN}[DATA] Use options 5,6,7 to review your collected intelligence${NC}"
            exit 0 
            ;;
        *) 
            echo -e "${RED}[ERROR] Invalid selection, you fucking moron${NC}"
            ;;
    esac
    
    echo ""
    echo -n -e "${YELLOW}Press enter to continue...${NC}"
    read
done
EOF

    chmod +x "$MAIN_DIR/LAUNCH_ME.sh"
    echo "[SUCCESS] Enhanced launcher with data review created"
}

# Build network scanner for completeness
build_network_scanner() {
    cat > "$MAIN_DIR/tools/scripts/network_scanner.sh" << 'EOF'
#!/bin/bash
# POPS Network Scanner

SCAN_DIR="../../data/scans/"
mkdir -p "$SCAN_DIR"

echo "[NETSCAN] POPS Network Scan - Output: $SCAN_DIR"

# Basic network info
date > "$SCAN_DIR/network_info.txt"
echo "=== NETWORK INFORMATION ===" >> "$SCAN_DIR/network_info.txt"
ifconfig 2>/dev/null || ip addr 2>/dev/null >> "$SCAN_DIR/network_info.txt"

echo "[NETSCAN] Scan complete. View with: ./LAUNCH_ME.sh then option 6"
EOF

    chmod +x "$MAIN_DIR/tools/scripts/network_scanner.sh"
}

# Build data exfiltration tool
build_data_exfiltration() {
    cat > "$MAIN_DIR/tools/scripts/data_exfil.py" << 'EOF'
#!/usr/bin/env python3
import os
import zipfile
from datetime import datetime

class POPSExfil:
    def create_exfil_package(self):
        print("[EXFIL] Creating data exfiltration package...")
        zip_path = f"../../data/exfil/pops_data_{datetime.now().strftime('%Y%m%d_%H%M%S')}.zip"
        
        with zipfile.ZipFile(zip_path, 'w') as zipf:
            for root, dirs, files in os.walk("../../data"):
                for file in files:
                    if not file.endswith('.zip'):
                        file_path = os.path.join(root, file)
                        zipf.write(file_path, os.path.relpath(file_path, "../../data"))
        
        print(f"[EXFIL] Package created: {zip_path}")

if __name__ == "__main__":
    POPSExfil().create_exfil_package()
EOF

    chmod +x "$MAIN_DIR/tools/scripts/data_exfil.py"
}

# Main deployment function
deploy_enhanced_pops() {
    echo -e "\n[INFO] Deploying enhanced POPS with complete data review..."
    
    create_pops_structure
    create_pops_readme
    download_pops_tools
    build_enhanced_keylogger
    build_data_review_tools
    build_network_scanner
    build_data_exfiltration
    create_enhanced_launcher
    
    echo -e "\n${RED}╔══════════════════════════════════════════════════════════════╗"
    echo -e "║          ENHANCED POPS DEPLOYMENT COMPLETE               ║"
    echo -e "║           WITH COMPLETE DATA REVIEW SYSTEM              ║"
    echo -e "╚══════════════════════════════════════════════════════════════╝${NC}"
    echo -e "${GREEN}[SUCCESS] Your fucking enhanced POPS suite is ready!${NC}"
    echo -e "${YELLOW}[LOCATION] $MAIN_DIR${NC}"
    echo -e "${CYAN}[DATA REVIEW] Run ./LAUNCH_ME.sh and use options 5,6,7${NC}"
    echo -e "${CYAN}[KEYSTROKES] Option 5: View live and captured keystrokes${NC}"
    echo -e "${CYAN}[ALL DATA] Option 6: Comprehensive data review${NC}"
    echo -e "${CYAN}[LIVE] Option 7: Real-time data monitoring${NC}"
    echo -e "\n${GREEN}All data is organized in POPS/data/ - you can review everything${NC}"
}

# Execute the fucking enhanced deployment
deploy_enhanced_pops
