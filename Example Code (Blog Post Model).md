public class BlogPost
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string Content { get; set; }
    public DateTime CreatedAt { get; set; } = DateTime.Now;

    // Additional properties, such as Author, Comments, etc.

    // Navigation property for related comments
    public ICollection<Comment> Comments { get; set; }
}
