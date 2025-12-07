---
layout: post
title: "How I Used Claude to Build This Jekyll Website"
date: 2024-12-07 19:00:00 +0700
categories: [Development, Tutorial]
tags: [Claude, AI, Jekyll, Website, Development]
excerpt: "A behind-the-scenes look at how I leveraged Claude AI to design, build, and customize this Jekyll-based personal website from scratch."
---

# How I Used Claude to Build This Jekyll Website

Building a personal website can be daunting, especially when you want something that looks professional but don't have extensive web development experience. That's where Claude AI came to the rescue! In this post, I'll share how I used Claude to create this entire Jekyll-based website.

## Why I Chose Jekyll + Claude

I wanted a simple, fast, and maintainable website that could be hosted for free on GitHub Pages. Jekyll seemed perfect, but I needed help with:
- Setting up the project structure
- Customizing the design
- Writing clean, maintainable code
- Understanding Jekyll's templating system

Claude turned out to be an excellent development partner for this project.

## The Development Process

### 1. Initial Setup
Claude helped me:
- Choose Jekyll as the right static site generator
- Set up the basic project structure
- Configure `_config.yml` with the right settings
- Create the initial Gemfile with necessary dependencies

```yaml
# Example of the _config.yml Claude helped me create
title: Luu Anh Tuan
email: anhtuanluu36@gmail.com
description: Personal website and portfolio of Luu Anh Tuan
baseurl: ""
url: "https://luuanhtuan.github.io"
```

### 2. Layout Customization
One of the biggest challenges was customizing the footer. I wanted a 2-column layout instead of the default 3-column. Claude helped me:
- Modify the `_includes/footer.html` template
- Update the corresponding SCSS styles in `_sass/_layout.scss`
- Ensure responsive design worked properly

### 3. Content Structure
Claude assisted with:
- Creating a logical page structure
- Writing the privacy policy content
- Setting up the blog post template
- Organizing navigation menus

### 4. Styling and Design
The visual improvements included:
- Custom CSS for better typography
- Responsive grid layouts
- Icon styling and positioning
- Color scheme adjustments

## Key Benefits of Using Claude

### 1. **Learning While Building**
Instead of just copying code, Claude explained each change:
- Why certain CSS properties were needed
- How Jekyll's templating works
- Best practices for file organization

### 2. **Problem Solving**
When I encountered issues like:
- Icons not aligning properly
- CSS not applying correctly
- Navigation not working as expected

Claude provided step-by-step solutions with explanations.

### 3. **Code Quality**
Claude helped ensure:
- Clean, readable code structure
- Proper commenting
- Following Jekyll conventions
- SEO-friendly markup

### 4. **Iterative Improvements**
The development process was highly iterative:
1. I'd describe what I wanted
2. Claude would implement it
3. We'd test and refine
4. Repeat until perfect

## Specific Examples

### Footer Redesign
**Original problem**: The default Minima theme had a 3-column footer that felt cluttered.

**Claude's solution**:
```scss
.footer-col-1 {
  width: calc(40% - (#{$spacing-unit} / 2));
}
.footer-col-2 {
  width: calc(60% - (#{$spacing-unit} / 2));
}
.footer-col-3 {
  display: none;
}
```

### Icon Styling
**Challenge**: GitHub icon was inheriting link colors and not aligning properly.

**Claude's approach**:
```scss
.svg-icon {
  width: 16px;
  height: 16px;
  display: inline-block;
  vertical-align: middle;
}
.social-media-list li a {
  display: flex;
  align-items: center;
  white-space: nowrap;
}
```

## Lessons Learned

1. **AI as a Development Partner**: Claude wasn't just a code generator—it was a thoughtful development partner that helped me understand each decision.

2. **Iterative Development**: Building in small, iterative steps with Claude's help was much more effective than trying to build everything at once.

3. **Documentation Matters**: Claude's explanations served as instant documentation for future reference.

4. **Best Practices**: Working with Claude ensured I followed Jekyll and web development best practices from the start.

## Tips for Using Claude in Web Development

### 1. Be Specific
Instead of: "Make it look better"
Try: "Change the footer to 2 columns with contact info on the left and description on the right"

### 2. Ask for Explanations
Always ask "why" to understand the reasoning behind code changes.

### 3. Test Incrementally
Make one change at a time and test it before moving to the next feature.

### 4. Review Generated Code
While Claude is excellent, always review and understand the code it generates.

## The Result

The final website features:
- ✅ Clean, professional design
- ✅ Responsive layout
- ✅ SEO-optimized structure
- ✅ Easy-to-maintain codebase
- ✅ Fast loading times
- ✅ GitHub Pages hosting

## What's Next?

Now that I have a solid foundation, I plan to:
- Add more blog posts about my projects
- Create project showcase pages
- Implement analytics
- Add search functionality

All of these future enhancements will likely involve Claude as my development partner!

## Conclusion

Using Claude to build this website was an incredibly positive experience. It felt like pair programming with an expert developer who never got tired of explaining things. The combination of AI assistance and human creativity resulted in a website that I'm truly proud of.

If you're considering building your own website, I highly recommend trying this approach. The key is treating Claude as a collaborative partner rather than just a code generator.

---

*Have questions about this process or want to share your own experience using AI for web development? Feel free to reach out!*