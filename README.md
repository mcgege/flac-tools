# flac-tools

These tools convert my own FLAC audio repository into a MP3 directory (my mobile devices won't play FLAC). I call the walker script by cron every night, but of course you can trigger it whenever you want. 


## Prerequisites

- [FLAC tools](https://xiph.org/flac/download.html)
- [LAME MP3 Encoder](http://lame.sourceforge.net/download.php)
- Perl Interpreter


## Installation

Copy the scripts into your favourite directory and adjust the file paths in the SETUP section of `flac2mp3` and `flac2mp3_walker`.


## Usage

`flac2mp3 <filename.flac>` converts a FLAC file into a MP3 file in the same directory.

`flac2mp3_walker` walks through your FLAC directory and looks for the corresponding MP3 files in a separate directory tree. If the file is missing, `flac2mp3` is called and the MP3 file (and if needed: the dir) is created. 


## License and Author

* Author: Michael Geiger <info@mgeiger.de>

Licensed under the GNU General Public License, Version 3 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

    http://www.gnu.org/licenses/gpl-3.0.html

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
