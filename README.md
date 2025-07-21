# Text-editor


<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jodit@3.24.3/build/jodit.min.css">

<textarea class="form-control editor" name="preparation_plans" rows="5" placeholder="Enter Details" required>{{ $course->preparation_plans }}</textarea>
<script src="https://cdn.jsdelivr.net/npm/jodit@3.24.3/build/jodit.min.js"></script>

<script>
    $(document).ready(function() {
        $('.editor').each(function() {
            new Jodit(this, {
                height: 300, // Adjust the editor height
                toolbarSticky: false, // Toolbar will not stick on scroll
                defaultMode: "1", // Start in WYSIWYG mode
                uploader: {
                    insertImageAsBase64URI: true // Allows direct image uploads
                }
            });
        });
    });
</script>
