# OE-3

class SocialMediaAccount():
     def __init__(self, username, password):
          self.username = username
          self.password = password
        
     def describeSocialMediaAccount(self):
          print(f"Account: {self.username}")

class InstagramAccount(SocialMediaAccount):
     def __init__(self, username, password, number_of_followers):
          super().__init__(username, password)
          self.number_of_followers = number_of_followers
          
     def share_story(self):
          print(f"{self.username} share story!")

ig = InstagramAccount("ayana", "nothingpass", 97)
ig.describeSocialMediaAccount()
print(f"Followers: {ig.number_of_followers}")
ig.share_story()

class TwitterAccount(SocialMediaAccount):
     def __init__(self, username, password, number_of_tweets): 
          super().__init__(username, password)
          self.number_of_tweets = number_of_tweets
          
     def tweet(self):
          print(f"{self.username} private tweet!")
          
tweet = TwitterAccount("yanasorr", "keepsilence", 0)
tweet.describeSocialMediaAccount()
print(f"Tweets: {tweet.number_of_tweets}")
tweet.tweet()
