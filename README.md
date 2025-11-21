# Bangkok Cam - Sukhumvit Live Stream

Live webcam streaming Sukhumvit Road in Bangkok, Thailand.

## Tech Stack
- **go2rtc** - RTSP to WebRTC conversion
- **nginx** - Web server
- **Docker Compose** - Container orchestration
- **Cloudflare** - CDN and DNS

## Environment Variables

Set these in Coolify:

- `CAMERA_PASSWORD` - Password for the Tapo camera account

## Deployment

This repo is deployed via Coolify on a VPS.

### Prerequisites
1. Port forward 8554 on home router to camera (192.168.1.200:554)
2. Set up DDNS for home.bangkokcam.com
3. Configure Cloudflare DNS

### Coolify Setup
1. Connect this GitHub repo
2. Add environment variable `CAMERA_PASSWORD`
3. Set domain to bangkokcam.com
4. Deploy!

## Local Development
```bash
