<script>
    let story = {
        score: 0,
        title: "First story",
        user: {
            username: 'user'
        },
        link: '/story/123',
        commentCount: '2 Comments',
        createdAt: '2 days ago'
    }
</script>

<div class="hompage page">
    <div class="story-item">

        <div class="voter">
            <span class="upvoter">
                <span class="arrow"></span>
            </span>
            <span class="score">{story.score}</span>
        </div>

        <div class="main">
            <div class="details">
                <a class="title" href={story.link}>{story.title}</a>
                <span class="domain">self</span>
            </div>
            <div class="byline">
                by {story.user.username} {story.createdAt} | 
                <a class="comments-link" href={story.link}>{story.commentCount}</a>
            </div>
        </div>
    </div>
</div>