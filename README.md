# Google Colab Torrent Client

![Torrent Download](https://img.shields.io/badge/Downloads-Torrents-blue) ![Google Colab](https://img.shields.io/badge/Platform-Google_Colab-orange) ![Drive Storage](https://img.shields.io/badge/Storage-Google_Drive-green)

A secure torrent client running in Google Colab that downloads files directly to your Google Drive via magnet links, with selective file downloading and real-time progress monitoring.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1h9uWkkZPaEuyczgYW-uagF5JjaP4F8Yk)

## Features ✨

- 🚀 **Google Drive Integration** - Direct downloads to your Drive
- 🔍 **Metadata Fetching** - Retrieve torrent info before download
- ✔️ **File Selection** - Choose specific files from torrents
- 📊 **Real-time Progress** - Visual progress bars & speed stats
- 🌐 **DHT Support** - Better peer discovery through distributed hash table
- 🧹 **Auto-cleanup** - Removes .parts files after completion
- ⏸️ **Resume Support** - Save session state for interruptions

## Prerequisites 📋

- Google Account
- Google Drive storage space
- Basic understanding of magnet links
- Colab runtime access

## Usage Steps 🛠️

1. **Run the script** in [Colab](https://colab.research.google.com/)
2. **Paste magnet link** when prompted
3. **Select files** using:
   - Individual numbers (0,2,5)
   - Ranges (0-4)
   - **Both** individual *and* ranges (2-4,8,12-18)
   - 'all' or 'none'
4. **Monitor progress** with live stats:
   ```plaintext
   Torrent: Totally Legal Torrent! (Save: /content/drive/MyDrive/TorrentDownloads)
   Overall Progress (Selected): [░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 0.00%
   Status: downloading
   ----------------------------------------------------------------------
   Individual File Progress:
   - Totally Legal Torrent!/Totally Legal File.mkv
   [░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 0.00/399.33MB (0.0%)
   ----------------------------------------------------------------------
   Peers: 12 (Seeds: 10, Conns: 57, DHT: 62)
   DL Speed: 144.21 KB/s | UL Speed: 0.00 KB/s
   Total Selected Downloaded: 0.00 MB / 399.33 MB
   ETA (Selected): 00:47:15
   Elapsed Time: 00:00:15
   ```
5. **Default Download Path** (`save_path`): `'/content/drive/MyDrive/TorrentDownloads'`

## Important Notes ⚠️

- **Runtime Limits**: Colab sessions disconnect after ~12h
- **Network Restrictions**: May not work in region-restricted networks
- **File Conflicts**: Avoid duplicate filenames in Drive
- **Speed Variability**: Depends on Colab's network & torrent health

## Disclaimer 🛑

❗ **Use responsibly** - Only download content you have legal rights to access.  
🔒 **Security** - This script doesn't persist any download history after session end.  
⚠️ **No Warranty** - Use at your own risk. Maintainer not responsible for data loss or misuse.
