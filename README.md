# NTR

*This fork is for my personal use at the monment as others work on improving the overall NTR code.*

Changes I made:
- Replaced screenshot index naming scheme with a timestamp one.
	- Now it doesn't need to scan the full directory for the index on boot, much faster boot time when there are a lot of screenshots.
- Changed screenshot directory to /Screenshots
	- The old libctru version NTR uses right now doesn't have `CreateDirectory` in `fs`, so screenshots will not save unless /Screenshots directory is present on the SD card.
- Changed screenshot default hotkey to Select+Start
- Changed top screen color signal to bottom screen
- Shortened screenshot color signal time by 10x
- Added top screen only screenshot hotkey L+R

# TODO LIST

0. Fix the build system first.
1. The printf impl. (xprintf.c) is not thread-safe, it should be replaced with a thread-safe one.

# LICENSE 

GPLv2
