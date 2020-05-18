import random
import plexapi

plex_url = 'https://plexurl'
plex_token = 'token'

from plexapi.server import PlexServer
plex = PlexServer(plex_url, plex_token)
videos = plex.library.section('Movies').search("")
print("Found %d Videos" % len(videos))
choice = random.choice(videos)
print("Selected " + choice.title)
video_url = choice.getStreamURL()
print(video_url)
