<template>
<div id="chat-container" class="d-flex flex-column">
    <!-- Breadcrumb -->
    <div aria-label="breadcrumb" class="d-flex justify-content-between" id="chat-breadcrumb">
        <div class="fw-bold">Chat</div>
        <div>
            <ol class="breadcrumb m-0">
                <li class="breadcrumb-item"><i class="bi bi-house"></i></li>
                <li class="breadcrumb-item active" style="color:#635BFF" aria-current="page">Chat</li>
            </ol>
        </div>
    </div>

    <div id="chat-content" class="d-flex flex-grow-1">
        <!-- Messages List -->
        <div id="chat-list" class="border-end">
            <ul class="list-unstyled">
                <li class="p-2 fw-bold"><img src="@/assets/avatar.svg" alt="user">
                    Mathew Anderson <button id="dots" class="border-0 btn btn-white"><i class="bi bi-three-dots-vertical"></i></button>
                    <br><small>Marketing Director</small></li>
            </ul>
            <div class="input-group input-group-sm">
                <button class="btn btn-light border border-end-0"><i class="bi bi-search fs-6"></i></button>
                <input type="text" class="form-control" placeholder="Search Contacts">
            </div>
            <p class="mt-3" style="color:#98A4AE;">Recent Chats <i class="bi bi-chevron-down"></i></p>
            <ul class="list-unstyled">
                <li class="p-2 mb-1 fw-bold" style="background-color: #eaeef0;">
                    <div class="d-flex">
                        <div><img style="height: 37px;" src="@/assets/avatar1.svg" alt="user1"></div>
                        <div class="mt-4" style="margin-left: -6px;"><img src="@/assets/onlin.svg/" alt=""></div>
                        <div class="fw-bold">Michell Flintoff<small class="ps-3">15 min You: Yesterday was great...</small></div>
                    </div>
                </li>

                <li class="p-2 mb-1 fw-bold">
                    <div class="d-flex">
                        <div><img style="height: 37px;" src="@/assets/avatar2.svg" alt="user2"></div>
                        <div class="mt-4" style="margin-left: -6px;"><img src="@/assets/offline.svg/" alt=""></div>
                        <div class="fw-bold">Bianca Anderson<small>30 min Nice looking dress you...</small></div>
                    </div>
                </li>
                <li class="p-2 mb-1 fw-bold">
                    <div class="d-flex">
                        <div><img style="height: 37px;" src="@/assets/avatar3.svg" alt="user3"></div>
                        <div class="mt-4" style="margin-left: -6px;"><img src="@/assets/yellow.svg/" alt=""></div>
                        <div class="fw-bold">Michell Flintoff<small class="ps-3">15 min You: Yesterday was great...</small></div>
                    </div>
                </li>
                <li class="p-2 mb-1 fw-bold">
                    <div class="d-flex">
                        <div><img style="height: 37px;" src="@/assets/avatar4.svg" alt="user4"></div>
                        <div class="mt-4" style="margin-left: -6px;"><img src="@/assets/onlin.svg/" alt=""></div>
                        <div class="fw-bold">Andrew Johnson<small>2 hours Sent a photo</small></div>
                    </div>
                </li>
                <li class="p-2 mb-1 fw-bold">
                    <div class="d-flex">
                        <div><img style="height: 37px;" src="@/assets/avatar5.svg" alt="user5"></div>
                        <div class="mt-4" style="margin-left: -6px;"><img src="@/assets/onlin.svg/" alt=""></div>
                        <div class="fw-bold">Mark, Stoinus& Ri<small>15 min Lorem ipsum text</small></div>
                    </div>
                </li>
            </ul>
        </div>

        <!-- Chat Window -->
        <div id="chat-messages" class="flex-grow-1 p-2 d-flex flex-column">
            <ul class="list-unstyled">
                <li class="p-2 pt-0 border-bottom" style="color: #98A4AE;"><img style="border-radius: 50%; background-color: #D4FFD4; height: 37px;" src="@/assets/avatar1.svg" alt="away">
                    Away
                    <button type="button" class="border-0 btn btn-white" data-bs-toggle="modal" data-bs-target="#exampleModal" style="margin-left: 106px;"><i class="bi bi-slash-circle" style="color:#575CD4; font-size: 18px;"></i></button>
                    <button type="button" class="border-0 btn btn-white" data-bs-toggle="modal" data-bs-target="#exampleModaldelete"><i class="bi bi-trash" style="color:red; font-size: 18px;"></i></button>
                    <button type="button" class="border-0 btn btn-white" data-bs-toggle="modal" data-bs-target="#exampleModalUnlock"><i class="bi bi-telephone" style="font-size: 18px;"></i></button>
                    <button class="border-0 btn btn-white"><i class="bi bi-camera-video" style="font-size: 18px;"></i></button>
                    <button class="border-0 btn btn-white"><i class="bi bi-list" style="font-size: 18px;"></i></button></li>
            </ul>

            <div class="flex-grow-1 overflow-auto">
                <!-- Received Message -->
                <div class="d-flex align-items-center mb-1">
                    <img src="@/assets/avatar3.svg" style="height:30px" alt="">
                    <div class="ps-1" style="color:#98A4AE; font-size:10px;">Andrew, 2 hours ago</div>
                </div>
                <div class="message received d-flex mb-2">
                    <div class="message-content p-2 rounded">
                        If I don’t like something, I’ll stay away from it
                    </div>
                </div>
                <!-- Sent Message -->
                <div class="ps-1 text-end" style="color:#98A4AE; font-size:10px;">2 hours ago</div>
                <div class="message sent d-flex justify-content-end mb-2">
                    <div class="message-content text-black p-2 rounded">
                        If I don’t like something, I’ll stay away from it
                    </div>
                </div>
                <!-- Received Message -->
                <div class="d-flex align-items-center mb-1">
                    <img src="@/assets/avatar3.svg" style="height:30px" alt="">
                    <div class="ps-1" style="color:#98A4AE; font-size:10px;">Andrew, 2 hours ago</div>
                </div>
                <div class="message received d-flex mb-2">
                    <div class="message-content p-2 rounded">
                        I want more detailed information
                    </div>
                </div>
                <!-- Sent Message -->
                <div class="ps-1 text-end" style="color:#98A4AE; font-size:10px;">2 hours ago</div>
                <div class="message sent d-flex justify-content-end mb-2">
                    <div class="message-content text-black p-2 rounded">
                        They got there early, and they got really good seats
                    </div>
                </div>

                <!-- Received Message -->
                <div class="d-flex align-items-center mb-1">
                    <img src="@/assets/avatar3.svg" style="height:30px" alt="">
                    <div class="ps-1" style="color:#98A4AE; font-size:10px;">Andrew, 2 hours ago</div>
                </div>
                <div class="message received d-flex mb-2">
                    <div class="p-3">
                        <img src="@/assets/chatpic.png" style="height: 70px; border-radius: 4px;">
                    </div>
                </div>
            </div>

            <!-- Chat Input -->
            <div id="chat-input" class="p-0 border-top d-flex align-items-center">
                <div class="input-group">
                    <button class="btn btn-white"><i class="bi bi-emoji-smile fs-5"></i></button>
                    <input type="text" class="form-control border-0" placeholder="Type a Message">
                    <button class="btn btn-white"><i class="bi bi-image fs-5"></i></button>
                    <button class="btn btn-white"><i class="bi bi-paperclip fs-5"></i></button>
                    <button class="btn btn-white"><i class="bi bi-mic fs-5"></i></button>
                </div>
            </div>
        </div>

        <!-- Extra Column -->
        <div id="extra-column" class="p-1 border-start">
            <h6 class="p-2 ms-2">Media <span style="color: #98A4AE;">(36)</span></h6>
            <img src="@/assets/content.png" class="ms-2" alt="content" style="height:100px;">
            <h6 class="p-2 m-2">Files <span style="color: #98A4AE;">(36)</span></h6>
            <ul class="list-unstyled ms-3">
                <li class="mb-2">
                    <div class="d-flex">
                        <div class="me-1"><img src="@/assets/file1.png" style="height:34px; border-radius: 10px;"></div>
                        <div style="font-weight: bold; font-size: small;">service-task.pdf<br><small class="ms-0">2 MB 2 Dec 2022</small></div>
                    </div>
                </li>
                <li class="mb-2">
                    <div class="d-flex">
                        <div class="me-1"><img src="@/assets/file2.png" style="height:34px; border-radius: 10px;"></div>
                        <div style="font-weight: bold; font-size: small;">homepage-design.fig<br><small class="ms-0">2 MB 2 Dec 2022</small></div>
                    </div>
                </li>
                <li class="mb-2">
                    <div class="d-flex">
                        <div class="me-1"><img src="@/assets/file3.png" style="height:34px; border-radius: 10px;"></div>
                        <div style="font-weight: bold; font-size: small;">about-us.html<br><small class="ms-0">2 MB 2 Dec 2022</small></div>
                    </div>
                </li>
                <li class="mb-2">
                    <div class="d-flex">
                        <div class="me-1"><img src="@/assets/file4.png" style="height:34px; border-radius: 10px;"></div>
                        <div style="font-weight: bold; font-size: small;">work-project.zip<br><small class="ms-0">2 MB 2 Dec 2022</small></div>
                    </div>
                </li>
                <li>
                    <div class="d-flex">
                        <div class="me-1"><img src="@/assets/file5.png" style="height:34px; border-radius: 10px;"></div>
                        <div style="font-weight: bold; font-size: small;">custom.js<br><small class="ms-0">2 MB 2 Dec 2022</small></div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</div>

<!-- Block Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog modal-sm">
        <div class="modal-content">
            <div class=" mb-0 pb-0 modal-body text-center align-items-center">
                <i class="bi bi-slash-circle fw-bold" style="color:#575CD4; font-size: 25px;"></i>
                <h6>Block User</h6>
                <p style="font-size: small;" class="text-muted">You Are Going To Block This User Are You Sure?</p>
            </div>
            <div class="modal-footer justify-content-center border-top-0">
                <button type="button" class="btn border-0" style="width: 95px; color: white; background-color:#959595;" data-bs-dismiss="modal">Cancel</button>
                <button type="button" class="btn" style="color:white; width: 95px; background-color:#575CD4;">Yes</button>
            </div>
        </div>
    </div>
</div>

<!-- Delete Modal -->
<div class="modal fade" id="exampleModaldelete" tabindex="-1" aria-labelledby="exampleModaldeleteLabel" aria-hidden="true">
    <div class="modal-dialog modal-sm">
        <div class="modal-content">
            <div class=" mb-0 pb-0 modal-body text-center align-items-center">
                <i class="bi bi-trash fw-bold" style="color:#575CD4; font-size: 25px;"></i>
                <h6>Delete Conversation</h6>
                <p style="font-size: small;" class="text-muted">Once You Sure To Delete This Conversation, You Will Not Be Able To Undo This Action</p>
            </div>
            <div class="modal-footer justify-content-center border-top-0">
                <button type="button" class="btn border-0" style="width: 95px; color: white; background-color:#959595;" data-bs-dismiss="modal">Cancel</button>
                <button type="button" class="btn" style="color:white; width: 95px; background-color:#575CD4;">Yes</button>
            </div>
        </div>
    </div>
</div>

<!-- Unlock Modal -->
<div class="modal fade" id="exampleModalUnlock" tabindex="-1" aria-labelledby="exampleModalUnlockLabel" aria-hidden="true">
    <div class="modal-dialog modal-sm">
        <div class="modal-content">
            <div class=" mb-0 pb-0 modal-body text-center align-items-center">
                <i class="bi bi-unlock fw-bold" style="color:#575CD4; font-size: 25px;"></i>
                <h6>Unlock User</h6>
                <p style="font-size: small;" class="text-muted">You Are Going To Unblock This User, Are You Sure?</p>
            </div>
            <div class="modal-footer justify-content-center border-top-0">
                <button type="button" class="btn border-0" style="width: 95px; color: white; background-color:#959595;" data-bs-dismiss="modal">Cancel</button>
                <button type="button" class="btn" style="color:white; width: 95px; background-color:#575CD4;">Yes</button>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
#chat-container {
    position: fixed;
    top: 60px;
    left: 230px;
    right: 20px;
    bottom: 20px;
    background: #F4F7FB;
    display: flex;
    flex-direction: column;
    border-radius: 10px;
    padding: 17px;
}

#chat-breadcrumb {
    background: white;
    padding: 10px;
    border-radius: 10px;
    margin-left: 9px;
    margin-right: 9px;
}

#chat-content {
    display: flex;
    flex-grow: 1;
    margin: 9px;
    border-radius: 10px;
    background: white;
    padding: 10px;
    height: 90%;
}

#chat-list,
#extra-column {
    width: 260px;
    background: white;
    overflow-y: auto;
    padding: 5px;
}

.received .message-content {
    background: #EFF4FA;
    border-radius: 15px 15px 15px 0;
    height: 30px;
    font-size: 11px;

}

.sent .message-content {
    background: #ECFDFD;
    border-radius: 15px 15px 0 15px;
    height: 30px;
    font-size: 11px;
}

#chat-input {
    border-top: 1px;
    display: flex;
}

#chat-list li {
    width: 239px;
    height: 55px;
    font-size: small;
}

small {
    font-size: smaller;
    margin-inline-start: 40px;
    color: #98A4AE;
    font-weight: 400;
}

#dots {
    margin-left: 29px;
}
</style>
